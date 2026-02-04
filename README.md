// Me.ts
export class Me {}

// About.ts
import { Me } from './Me';

export class About extends Me {
  getPersonalInfo(): Record<string, string> {
    return {
      name: 'Raphael Alves de Oliveira',
      position: 'Software Architect',
      location: 'São Paulo, Brazil 🇧🇷',
      website: 'https://raphaeloliveiradev.netlify.app/'
    };
  }

  getSkills(): Record<string, string[]> {
    return {
      languages: ['JavaScript/TypeScript', 'PHP'],
      frameworks: ['React', 'WordPress', 'Express', 'Next.js', 'Fastify'],
      databases: ['MySQL', 'PostgreSQL', 'Firestore'],
      orm: ['Prisma']
    };
  }
}
