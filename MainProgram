using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows;
using System.Windows.Controls;
using System.Windows.Data;
using System.Windows.Documents;
using System.Windows.Input;
using System.Windows.Media;
using System.Windows.Media.Imaging;
using System.Windows.Navigation;
using System.Windows.Shapes;
using System.IO;
using System.Threading;

namespace fileWriter
{
    /// <summary>
    /// Interaction logic for MainWindow.xaml
    /// </summary>
    public partial class MainWindow : Window
    {
        public MainWindow()
        {
            InitializeComponent();
            string p = Environment.GetFolderPath(Environment.SpecialFolder.MyDocuments);
            System.IO.Directory.CreateDirectory(p + @"\textsaves");
            string fo = @"\textsaves";
            string fi = @"\text.txt";
            string pfo = p + fo;
            string pfi = pfo + fi;
            if (!File.Exists(pfi))
            {
                File.Create(pfi);
            }
        }

        private void Button_Click(object sender, RoutedEventArgs e)
        {
            string fo = @"\textsaves";
            string fi = @"\text.txt";
            string p = Environment.GetFolderPath(Environment.SpecialFolder.MyDocuments);
            string pfo = p + fo;
            string pfi = pfo + fi;
            string text = Convert.ToString(body.Text);
            File.AppendAllText(pfi, " Update: " + text);
        }
    }
}         
