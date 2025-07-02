import React, { useState } from 'react';
import {
  Github, Linkedin, Mail, Book, Code, Cpu, Database, Briefcase, Award, GraduationCap,
  Sparkles, Layers, GitBranch, Terminal, LayoutGrid, HardDrive, Factory, Lightbulb,
  ChevronDown, ChevronUp
} from 'lucide-react';

// Main App component for the GitHub README
function App() {
  const [activeCategory, setActiveCategory] = useState(null);

  // Function to toggle skill category visibility
  const toggleCategory = (category) => {
    setActiveCategory(activeCategory === category ? null : category);
  };

  // Define skill categories and their respective skills
  const skillCategories = [
    {
      name: 'Software & Programming',
      icon: <Code className="w-6 h-6 text-blue-500" />,
      skills: [
        'Python', 'C++', 'C Programming', 'Arduino', 'Raspberry Pi', 'MATLAB',
        'Unity', 'Unreal Engine', 'ROS', 'Embedded Systems', 'Figma', 'Flutter',
        'KiCad', 'NodeJs', 'SQL', 'Q#', 'C#', 'Java', 'JavaScript', 'HTML',
        'TypeScript', 'Web Application Development', 'LLM', 'Generative AI',
        'AI APIs', 'TensorFlow', 'PyTorch', 'Deep Learning', 'Neural Networks',
        'Computer Vision', 'Linux', 'Git', 'GitHub'
      ],
    },
    {
      name: 'Electronics & Circuit Design',
      icon: <Cpu className="w-6 h-6 text-green-500" />,
      skills: [
        'PCB Design & Layout', 'Analog/Digital Circuit Design', 'Power Electronics',
        'Battery Management Systems', 'RF Design', 'IoT', 'Hardware Software Co-Design',
        'Software Debugging', 'Quantum Entanglement Testing', 'Verilog', 'VHDL',
        'Signal Processing', 'Networking', 'Altium', 'Allegro'
      ],
    },
    {
      name: 'Data Analysis & Research',
      icon: <Database className="w-6 h-6 text-purple-500" />,
      skills: [
        'Python for Data Analysis', 'Statistics', 'LLM', 'Generative AI',
        'Neutron Scattering Tests', 'Quantum Entanglement Testing',
        'Data Collection & Analysis', 'Matplotlib', 'Tableau', 'NumPy',
        'Power BI', 'Splunk', 'Hadoop', 'Hive', 'Redis', 'Spark'
      ],
    },
    {
      name: 'Systems & Project Management',
      icon: <Briefcase className="w-6 h-6 text-red-500" />,
      skills: [
        'Project Management', 'Leadership', 'Systems Design', 'Heat Transfer',
        'Automation and Robotics', 'Agile', 'CRM', 'SalesForce', 'Product Management',
        'Rapid Prototyping', 'Test Infrastructure', 'Communication'
      ],
    },
    {
      name: '3D Printing & Manufacturing',
      icon: <Factory className="w-6 h-6 text-yellow-500" />,
      skills: [
        '3D Printing (SLA, DLP, LCD)', 'Soldering', 'CAD Design (Siemens NX, SolidWorks, Onshape)',
        'Micrometers', 'GD&T Blueprints', 'CMMs'
      ],
    },
  ];

  return (
    <div className="min-h-screen bg-gray-900 text-gray-200 font-inter p-4 sm:p-8 flex items-center justify-center">
      <div className="w-full max-w-4xl bg-gray-800 rounded-xl shadow-2xl p-6 sm:p-10 border border-gray-700">
        {/* Header Section */}
        <header className="text-center mb-10">
          <h1 className="text-4xl sm:text-5xl font-extrabold text-white mb-2">NADAV SHANUN</h1>
          <p className="text-xl sm:text-2xl text-blue-400 font-semibold mb-4">Electrical & Robotics Engineer | AI/ML Enthusiast</p>
          <div className="flex justify-center space-x-6">
            <a
              href="https://www.linkedin.com/in/nadavshanun/" // Replace with actual LinkedIn URL
              target="_blank"
              rel="noopener noreferrer"
              className="text-gray-300 hover:text-blue-500 transition-colors duration-300 transform hover:scale-110"
              aria-label="LinkedIn Profile"
            >
              <Linkedin className="w-8 h-8" />
            </a>
            <a
              href="mailto:na195633@ucf.edu"
              className="text-gray-300 hover:text-red-500 transition-colors duration-300 transform hover:scale-110"
              aria-label="Email"
            >
              <Mail className="w-8 h-8" />
            </a>
            <a
              href="https://github.com/your-github-profile" // Replace with actual GitHub URL
              target="_blank"
              rel="noopener noreferrer"
              className="text-gray-300 hover:text-purple-500 transition-colors duration-300 transform hover:scale-110"
              aria-label="GitHub Profile"
            >
              <Github className="w-8 h-8" />
            </a>
          </div>
        </header>

        {/* About Me Section */}
        <section className="mb-10 p-6 bg-gray-700 rounded-lg border border-gray-600">
          <h2 className="text-3xl font-bold text-white mb-4 flex items-center">
            <Book className="w-7 h-7 mr-3 text-cyan-400" /> About Me
          </h2>
          <p className="text-lg leading-relaxed text-gray-300">
            Motivated Electrical Engineering major with an active Top Secret Security Clearance, passionate about
            innovating at the intersection of robotics, AI, and hardware. I thrive on developing cutting-edge solutions
            from concept to deployment, with a strong background in embedded systems, AI/ML, and project leadership.
            Committed to building impactful technologies that push the boundaries of what's possible.
          </p>
        </section>

        {/* Experience Highlights Section */}
        <section className="mb-10 p-6 bg-gray-700 rounded-lg border border-gray-600">
          <h2 className="text-3xl font-bold text-white mb-4 flex items-center">
            <Layers className="w-7 h-7 mr-3 text-orange-400" /> Experience Highlights
          </h2>
          <ul className="list-disc list-inside text-lg text-gray-300 space-y-3">
            <li>
              <span className="font-semibold text-white">NASA Electrical and Robotics Engineer Intern:</span> Developed haptic glove robotic systems for astronaut VR training and enhanced hardware functionality for an Iron Man style robotic haptic hand.
            </li>
            <li>
              <span className="font-semibold text-white">Department of Defense Nuclear and Electrical Engineer:</span> Developed microelectronics for thermonuclear warheads and created an AI API for atomic simulations.
            </li>
            <li>
              <span className="font-semibold text-white">Co-Founder and CTO, OnLife Startup:</span> Founded a company integrating health apps, directing a team of 11 employees and 35 interns, focusing on hardware solutions and mobile app development.
            </li>
            <li>
              <span className="font-semibold text-white">Co-Founder & CEO, PrecisionMed AI:</span> Developed and launched an AI-driven platform for personalized chemotherapy and led partnerships with hospitals.
            </li>
          </ul>
        </section>

        {/* Education Section */}
        <section className="mb-10 p-6 bg-gray-700 rounded-lg border border-gray-600">
          <h2 className="text-3xl font-bold text-white mb-4 flex items-center">
            <GraduationCap className="w-7 h-7 mr-3 text-teal-400" /> Education
          </h2>
          <p className="text-lg text-gray-300">
            <span className="font-semibold text-white">University of Central Florida</span> <br />
            B.S. in Electrical Engineering (Major GPA 3.8, Spring 2026) <br />
            Certificate: Engineering Leadership <br />
            Minors: Business Administration, Computer Science <br />
            <span className="font-semibold text-white">Active Top Secret Security Clearance</span>
          </p>
        </section>

        {/* Skills Section - Interactive */}
        <section className="mb-10 p-6 bg-gray-700 rounded-lg border border-gray-600">
          <h2 className="text-3xl font-bold text-white mb-4 flex items-center">
            <Sparkles className="w-7 h-7 mr-3 text-pink-400" /> My Skills
          </h2>
          <div className="space-y-4">
            {skillCategories.map((category) => (
              <div key={category.name} className="bg-gray-800 rounded-lg p-4 border border-gray-700">
                <button
                  className="w-full flex justify-between items-center text-left text-xl font-semibold text-white hover:text-blue-400 transition-colors duration-300"
                  onClick={() => toggleCategory(category.name)}
                >
                  <span className="flex items-center">
                    {category.icon}
                    <span className="ml-3">{category.name}</span>
                  </span>
                  {activeCategory === category.name ? (
                    <ChevronUp className="w-6 h-6" />
                  ) : (
                    <ChevronDown className="w-6 h-6" />
                  )}
                </button>
                {activeCategory === category.name && (
                  <div className="mt-4 pt-4 border-t border-gray-700">
                    <div className="flex flex-wrap gap-2 text-gray-300">
                      {category.skills.map((skill) => (
                        <span
                          key={skill}
                          className="bg-gray-600 px-3 py-1 rounded-full text-sm font-medium hover:bg-blue-600 transition-colors duration-200 cursor-default"
                        >
                          {skill}
                        </span>
                      ))}
                    </div>
                  </div>
                )}
              </div>
            ))}
          </div>
        </section>

        {/* Awards & Certificates Section */}
        <section className="mb-10 p-6 bg-gray-700 rounded-lg border border-gray-600">
          <h2 className="text-3xl font-bold text-white mb-4 flex items-center">
            <Award className="w-7 h-7 mr-3 text-yellow-400" /> Awards & Certificates
          </h2>
          <ul className="list-disc list-inside text-lg text-gray-300 space-y-2">
            <li>Omicron Delta Kappa National Leadership Honor Society</li>
            <li>Yale University Certificate in Connected Leadership</li>
            <li>Google Certificate: Large Language Models</li>
            <li>NVIDIA Generative AI Certification</li>
            <li>RF Design, PCB Design, Generative AI Certificates</li>
          </ul>
        </section>

        {/* What I'm Currently Working On (Example) */}
        <section className="mb-10 p-6 bg-gray-700 rounded-lg border border-gray-600">
          <h2 className="text-3xl font-bold text-white mb-4 flex items-center">
            <GitBranch className="w-7 h-7 mr-3 text-lime-400" /> What I'm Currently Working On
          </h2>
          <p className="text-lg leading-relaxed text-gray-300">
            Currently deep diving into advanced AI models for real-time robotic control and exploring new frontiers in quantum computing applications for aerospace. Always eager to collaborate on innovative projects!
          </p>
        </section>

        {/* Connect with Me Section */}
        <section className="p-6 bg-gray-700 rounded-lg border border-gray-600">
          <h2 className="text-3xl font-bold text-white mb-4 flex items-center">
            <Lightbulb className="w-7 h-7 mr-3 text-indigo-400" /> Let's Connect!
          </h2>
          <p className="text-lg text-gray-300 mb-4">
            Feel free to reach out if you'd like to discuss potential collaborations, exciting projects, or just chat about technology!
          </p>
          <div className="flex flex-wrap gap-4 justify-center">
            <a
              href="https://www.linkedin.com/in/nadavshanun/"
              target="_blank"
              rel="noopener noreferrer"
              className="bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-6 rounded-lg flex items-center space-x-2 transition-all duration-300 transform hover:scale-105 shadow-lg"
            >
              <Linkedin className="w-6 h-6" />
              <span>Connect on LinkedIn</span>
            </a>
            <a
              href="mailto:na195633@ucf.edu"
              className="bg-red-600 hover:bg-red-700 text-white font-bold py-3 px-6 rounded-lg flex items-center space-x-2 transition-all duration-300 transform hover:scale-105 shadow-lg"
            >
              <Mail className="w-6 h-6" />
              <span>Send an Email</span>
            </a>
          </div>
        </section>
      </div>
    </div>
  );
}

export default App;
