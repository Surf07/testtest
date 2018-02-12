using UnityEngine;
using System.Collection;

public class CubeController : MonoBehaviour {

public float speed = 1f;

void Start ( )  {
}

void Update ( ) {

Vector3 move = new Vector3 (

Input.GetAxis ("Horizontal"), 0, Input.GetAxis (" Vertical") )+
transform.Translate ( move * Time.deltaTime * speed) ;

}
}
}





Test Test OK?


importUIkit

import SpriteKit
import GameplayKit

class GameViewController: UIViewController {

override func viewDidLoad() {
super.viewDidLoad()

if let view = self.view as! SKView? {
// Load the SKScene from 'GameScene.sks'
if let scene = SKScene(fileNamed: "GameScene") {
// Set the scale mode to scale to fit the window
scene.scaleMode = .aspectFill

// Present the scene
view.presentScene(scene)
}

view.ignoresSiblingOrder = true

view.showsFPS = true
view.showsNodeCount = true
}
}

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
