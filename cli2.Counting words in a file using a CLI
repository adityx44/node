import {program} from 'commander';
import chalk from 'chalk';
import fs from 'fs';
program
 .name('Count words')
 .description('CLI to count no. of words')
 .version('1.0.0')
 .argument('<file>','file to count')
 .action((file)=>{
    fs.readFile(file,'utf-8',(err,data)=>{
        if(err)
        {
            console.log(err);
        }
        else{
            const words=data.split(/\s+/).length;
            console.log(chalk.blue( `There are ${words} words in ${file}`));
        }
    });
 });
 program.parse();

