# basic-animation-loops
[![Watch the video](https://img.youtube.com/vi/VIDEO_ID/maxresdefault.jpg)](https://github.com/user-attachments/assets/dab784ca-fb88-4bc7-a197-d451b0406ce0)



C# .Net Framework code

        private void DrawSomething(object sender, PaintEventArgs e)
        {
            Pen pen = new Pen(Color.Blue, 5);
            int Counter = 50;
            int intkoko = 0;
            while (true)
            {
                if(intkoko>=10000000)
                {
                    e.Graphics.Clear(this.BackColor);
                    e.Graphics.DrawLine(pen, Counter-20, 200, Counter, 200);
                    e.Graphics.DrawLine(pen, Counter - 20, 250, Counter, 250);
                    
                    e.Graphics.DrawLine(pen, 100,Counter - 20, 100, Counter);
                    e.Graphics.DrawLine(pen, 150, Counter - 20, 150, Counter);

                    Counter += 20;
                    intkoko = 0;

                }
                intkoko++;
                if (Counter >= 400)
                    Counter = 50;

            }
