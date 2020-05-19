# AFAR: Assisted Focus Audio Reviewer

AFAR (Assisted Focus Audio Reviewer) is a web application that transcribes in real-time audio inputs from a microphone attached to a speaker so that the user can read follow along with the speaker while wearing noise-canceling headphones to filter out the noise distractions. This allows the user to be either in a separate, distraction-free room or in the same room as the speaker but able to focus on the lecture.

### To run locally:

Please install python3 and pyaudio using pip. You may also need to install portaudio using your os package manager (e.g. Homebrew for MacOS). Execute run.sh as root to deploy the application locally. Please check setup.py for additional dependencies.

### Tech stack:
Made with Python, using jQuery, Bootstrap, Socket.io, Quill, Flask, flask-socket.io, rev.ai

### Inspiration:

There are students and learners in my community who struggle with ADHD and focusing in open, noisy environments. It inspired me to build an application that would be able to help users with focusing issues read and listen to verbal presentations while filtering out the noise and audible distractions. This technology helps not just those who are neuro-atypical but alsp people with learning disabilities.

### Putting it together:

I used the rev.ai API speech-to-text service to record the microphone input of the speaker and the Streaming Speech-To-Text API to make API calls through sockets and displaying the transcript of the transcribed text on our front-end. The transcript works as note-taking for the class with the implemented annotation features of a text editor. The app uses Quill which is a free, open-source WYSIWYG editor built for web apps. To facilitate better learning, the students can also have the lecture content along with their notes read out to them in a generic and easy to understand voice. I implemented this by using the SpeechSynthesis API. Listening, transcribing, and note-taking at their own pace provides a simpler and enriching learning experience for everyone, regardless of their abilities.


