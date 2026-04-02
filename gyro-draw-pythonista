from scene import *
import motion

class Game(Scene):
	def setup(self):
		self.background_color = False
		fill('white')
		self.ptx = 180
		self.pty = 310
		
	def draw(self):
		self.a = SpriteNode('plf:Enemy_SlimeBlock', position=(self.ptx, self.pty),
		size=(1,1))
		self.add_child(self.a)
		
	def update(self):
		motion.start_updates()
		x, y, z = motion.get_gravity()
		self.ptx += x*8
		self.pty += y*8

if __name__ == '__main__':
	run(Game(),PORTRAIT,show_fps=True)
