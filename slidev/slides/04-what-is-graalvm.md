# What is GraalVM?

&nbsp;

**GraalVM Architecture**

- ð¹ï¸ Java HotSpot VM
- ð­ GraalVM compiler (JIT Compiler)[^1]
- ð Truffle Language Implemention Framework

<img
  v-click="1" class="example-image" 
  src="https://www.graalvm.org/docs/img/graalvm_architecture_community.png"
/>

<div v-click="2">

**Runtime Mode**

- JVM Runtime Mode
- Native Image
- <span class="emphasize-text">Java On Truffle (experimental)</span>
  - `java -truffle [options] class`
  - `java -truffle --java.JavaHome=/path/to/java/home -version`

</div>

[^1]: 1.[ Javac Compiler vs JIT Compiler](/images/compiler.jpg)

<style>

.example-image {
  position: absolute;
  top: 120px;
  right: 0px;
  width: 510px;
}

</style>

<!--

GraalVM compiler(jit):

sourcecode  ->  bytecode  ->  machine code

 ââââ javac ââââ   ââââ jit âââââ

Truffle Framework: implemnets by graalvm

jvm run time mode: java code éè¿é¡¶çº§ç¼è¯å¨(graalvm compiler)ç¼è¯ç´æ¥è¿è¡å¨jvmä¸, å¶ä»è¯­è¨éè¿truffleæ¦æªå¹¶è§£æåè¿è¡å¨vmä¸­

native image: æ¯ä¸é¡¹åæ°ææ¯, å°java bytecode ç¼è¯ä¸ºæ§è¡æä»¶

java on truffle: 21.0.0 å®éªçæ¬, æ¯ä¸ä¸ªå®æ´ç java èææºè§èå®ç°, åºäº truffle framework
- åç¬å®è£: gu install espresso / gu install -L espresso.jar
- run with truffle: java -truffle

-->
