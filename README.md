# xq-audio-player
Play audio online with http url
# Play http audio very simple code
Install manualy, you can copy XQAudioPlayer folder to your project. After that, using simple code to play a http audio url

        let audioPlayer = XQAudioPlayer.init(frame: CGRect(x: 0, y: 0, width: SCREEN_WIDTH, height: SCREEN_WIDTH * 0.3), urlString: url)
        self.view.addSubview(audioPlayer)
