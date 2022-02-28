# QR Code Generator and Reader.

 private void button1_Click(object sender, EventArgs e)
        {
            QRCodeEncoder enc = new QRCodeEncoder();
            pictureBox1.Image = enc.Encode(textBox1.Text);

        }

        private void button2_Click(object sender, EventArgs e)
        {
            QRCodeDecoder end = new QRCodeDecoder();
            textBox1.Text = end.Decode(new QRCodeBitmapImage(pictureBox1.Image as Bitmap));


        }
    }
    }
    

