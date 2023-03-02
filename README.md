- 👋 Hi, I’m Oluwayomi Timileyin
- 👀 I’m a full stack (PEAN, php, jquery, javascript, tyscript, mysql, html, css etc) web , mobile app  and blockchain developer
- 💞️ I’m looking to collaborate on any blockchain or web app project
- 📫 How to reach me on whatsapp +2348165266243

/// Salutation ////
@
function logSkills(...skills: Array<string>){
    return function (target: any, propertyKey: string, descriptor: PropertyDescriptor) {
        const originalMethod = descriptor.value;
        descriptor.value = function (...args: any[]) {
            console.log('I have advance experience and knowledge in the following tech skills:', skills.join(', '))
            return originalMethod.apply(this, args);
        }
        return descriptor;
   }
}

function logMail(target: any, propertyKey: string, descriptor: PropertyDescriptor) {
    const originalMethod = descriptor.value;
    descriptor.value = function (...args: any[]) {
        console.log('I will be glad working with you kinldy a send me mail oluwayomitimileyin1105@gmail.com');
        const result = originalMethod.apply(this, args);
        return result;
    }
    return descriptor;
}

function addName(target: any, propertyKey: string, descriptor: PropertyDescriptor) {
    const originalMethod = descriptor.value;
    descriptor.value = function (...args: any[]) {
        const name = 'Oluwayomi Timileyin';
        const newArgument = [[...args][0] += '\n' + name];
        const result = originalMethod.apply(this, newArgument);
        return result;
    }
    return descriptor;
}

class Salutation {

    @logSkills('Javascript', 'Nodejs', 'Typscript', 'Jquery', 'Angular', 'PHP', 'and more...')
    @logMail
    @addName
    
    logName(greeting_text: string): void {
        console.log(greeting_text);
    }

}

const _Salutation = new Salutation();
_Salutation.logName('Kind Regards');
   
  ///result 
  
I have advance experience and knowledge in the following tech skills: Javascript, Nodejs, Typscript, Jquery, Angular, PHP, and more...
I will be glad working with you kinldy a send me mail oluwayomitimileyin1105@gmail.com
Kind Regards
Oluwayomi Timileyin

  
  /// Language ///
  
  Typscript
  
  /// readme  ///
  
  Make sure to enable "experimentalDecorators" in your tsconfig if you want to play around it
  
  /// if you will like to ['drop a complain', 'request for a clearification or explanation', 'suggest best practices', 'and so on...'] kingly message me thanks
  
