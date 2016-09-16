# xq-audio-player
Play audio online with http url
# Play http audio using very simple code
Oder to install manualy, please copy XQAudioPlayer folder to your project. After that, using simple code under here to play a http audio url:
        
        let url = "http://www.stephaniequinn.com/Music/Allegro%20from%20Duet%20in%20C%20Major.mp3"
        let audioPlayer = XQAudioPlayer.init(frame: CGRect(x: 0, y: 0, width: SCREEN_WIDTH, height: SCREEN_WIDTH * 0.3), urlString: url)
        self.view.addSubview(audioPlayer)
# Control property of player
        // Change progress color
        audioPlayer.progressColor = UIColor.blueColor()
        
        // Change background progress color
        audioPlayer.progressBackgroundColor = UIColor.grayColor()
        
        // Change title time label color
        audioPlayer.timeLabelColor = UIColor.blackColor()
        
        // Change height of progress
        audioPlayer.progressHeight = 6
        
        // Change button play image
        audioPlayer.playingImage = UIImage(named:"icon_playing")
        audioPlayer.pauseImage = UIImage(named:"icon_pause")
        
        // Setting delegate
        audioPlayer.delegate = self
# Delegate

    /* Player did updated duration time
     * You can get duration time of audio in here
     */
    func playerDidUpdateDurationTime(player: XQAudioPlayer, durationTime: CMTime) {
        
    }
    
    /* Player did change time playing
     * You can get current time play of audio in here
     */
    func playerDidUpdateCurrentTimePlaying(player: XQAudioPlayer, currentTime: CMTime) {
        
    }
    
    // Player begin start
    func playerDidStart(player: XQAudioPlayer) {
        
    }
    
    // Player stoped
    func playerDidStoped(player: XQAudioPlayer) {
        
    }
    
    // Player did finish playing
    func playerDidFinishPlaying(player: XQAudioPlayer) {
        
    }

        
