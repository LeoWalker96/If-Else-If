# If-Else-If
import javax.swing.JOptionPane;
public class Average {
     public static void main(String[] args) {
           String numPeople = JOptionPane.showInputDialog("Enter number of people");
           Short shortnumPeople = Short.parseShort(numPeople);
           String numPlayers = JOptionPane.showInputDialog("Enter number of players");     
           Short shortnumPlayers = Short.parseShort(numPlayers);

      if (shortnumPeople>=10) {
             JOptionPane.showMessageDialog(null,"There's " + numPeople + " individuals divided into " +  ((shortnumPeople/2)-1) + " groups of 2 plus one group of " + ((shortnumPeople%2)+2));
    } else if (shortnumPeople>=3) {
             JOptionPane.showMessageDialog(null,"There's " + numPeople + " individuals divided into " +  ((shortnumPeople/3)-1) + " groups of 3 plus one group of " + ((shortnumPlayers%3)+3));
    } else {
             JOptionPane.showMessageDialog(null, "The number of people has to be at least 3.");
    }
      if (shortnumPlayers<=55 && shortnumPlayers>=11) {
             JOptionPane.showMessageDialog(null, "There's " + numPlayers + " players divided into " + shortnumPlayers/11 + " teams of 11 plus one team of " + ((shortnumPlayers%11)+11));     
    } else {
             JOptionPane.showMessageDialog(null, "There's " + numPlayers + " players divided into 1 group");
    }
  }
}
