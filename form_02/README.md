```cs
private void InitializeComponent()
{
    this.action = new System.Windows.Forms.Button();
    this.SuspendLayout();
    // 
    // action
    // 
    this.action.Location = new System.Drawing.Point(92, 62);
    this.action.Name = "action";
    this.action.Size = new System.Drawing.Size(75, 23);
    this.action.TabIndex = 0;
    this.action.Text = "実行";
    this.action.UseVisualStyleBackColor = true;
    this.action.Click += new System.EventHandler(this.action_Click);
    // 
    // Form1
    // 
    this.AutoScaleDimensions = new System.Drawing.SizeF(7F, 15F);
    this.AutoScaleMode = System.Windows.Forms.AutoScaleMode.Font;
    this.ClientSize = new System.Drawing.Size(800, 450);
    this.Controls.Add(this.action);
    this.Name = "Form1";
    this.StartPosition = System.Windows.Forms.FormStartPosition.CenterScreen;
    this.Text = "Form1";
    this.ResumeLayout(false);

}

#endregion

private Button action;
```

```cs
public Form1()
{
    InitializeComponent();
}

private void action_Click(object sender, EventArgs e)
{
    Console.WriteLine("こんにちは世界");
    string resultLine = Console.ReadLine() + "";
    Console.WriteLine(resultLine);
}
```

![image](https://user-images.githubusercontent.com/1501327/184061125-611e0e6c-3d87-49bd-90fb-0de3fa3162d8.png)
