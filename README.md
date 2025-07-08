package XandO;

import javax.swing.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

public class ButtonManager {
    public static void setAction(JButton btn, int cell, XandOGame game) {
        btn.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                game.handleMove(btn, cell);
            }
        });
    }
}
