

Test Test OK?


importUIkit
override var shouldAutorotate: Bool {
return true
}

override var supportedInterfaceOrientations: UIInterfaceOrientationMask {
if UIDevice.current.userInterfaceIdiom == .phone {
return .allButUpsideDown
} else {
return .all
}
}
