Download Link: https://assignmentchef.com/product/solved-cpe212-project02
<br>
<strong>                                                            </strong>







<h1>Project02 Goals</h1>

A          fundamental  software         engineering    skill     is         the      design,            implementation,        and      testing of         a software         component     that     must   be        integrated      into     a          larger  software         product.                      In        order  to do        this,     the      software         component     must   conform          to         a          previously      agreed upon   interface         format. As        part     of         this      assignment,    you      will      practice          this      skill     by        completing     the      specification  and implementation         of         <strong>several           classes</strong>           that     will      be        integrated      into     a          larger  software         product provided        by        the      instructor.                  Along  the      way     you      will      review basic   C++     programming and      Linux  file management  skills   required         for       successful       completion     of         CPE     212.

<h1>Project02 Overview</h1>

For      this      project,           you      will      <strong><em>complete</em></strong>        the      provided        partial C++     program         that     utilizes            classes and inheritance    to         model geometric       shapes.           Class   <strong>Shape</strong> is         an        abstract          base    class    used    to         model properties      common         to         all        shapes including        its        <strong>Color</strong>.             <strong>Shape</strong> includes          a          function          (<strong>area</strong>) that must   exhibit polymorphic  behavior         in         any      derived           classes.                       Class   <strong>Triangle</strong>        is         a          derived class    that     is         used    to         model properties      of         all        triangles.                    The     <strong>Triangle</strong>        class    inherits from    the      base    class    <strong>Shape</strong>.            Class   <strong>Rectangle</strong>      is         a          derived           class    that     is         used    to         model properties      of         all        rectangles.                  The     <strong>Rectangle</strong>      class    inherits           from    the      base    class    <strong>Shape</strong>.            The <strong>Project02_Materials.zip</strong>     file       includes          four     source code    files     and      a          <strong>makefile</strong>.

<table width="735">

 <tbody>

  <tr>

   <td width="110"><strong>Filename                  </strong></td>

   <td width="191"><strong>Project02_Materials.zip                  </strong></td>

   <td width="433"><strong>Description         </strong></td>

  </tr>

  <tr>

   <td width="110"><strong>main.cpp                  </strong></td>

   <td width="191">Included</td>

   <td width="433">Driver    program                  to              test          <strong>Shape</strong>,   <strong>Triangle</strong>,                and                  <strong>Rectangle</strong>              classes</td>

  </tr>

  <tr>

   <td width="110"><strong>shape.h </strong></td>

   <td width="191"><strong>Write     and          submit  this                  file           </strong></td>

   <td width="433">Specification         file            for            <strong>Shape</strong>    class</td>

  </tr>

  <tr>

   <td width="110"><strong>shape.cpp                  </strong></td>

   <td width="191">Included</td>

   <td width="433">Implementation  file            for            <strong>Shape</strong>    class</td>

  </tr>

  <tr>

   <td width="110"><strong>triangle.h                  </strong></td>

   <td width="191">Included</td>

   <td width="433">Specification         file            for            <strong>Triangle</strong>                 class</td>

  </tr>

  <tr>

   <td width="110"><strong>triangle.cpp                  </strong></td>

   <td width="191"><strong>Write     and          submit  this                  file</strong></td>

   <td width="433">Implementation  file            for            <strong>Triangle</strong>                 class</td>

  </tr>

  <tr>

   <td width="110"><strong>rectangle.h                  </strong></td>

   <td width="191">Included</td>

   <td width="433">Specification         file            for            <strong>Rectangle</strong>              class</td>

  </tr>

  <tr>

   <td width="110"><strong>rectangle.cpp                  </strong></td>

   <td width="191"><strong>Write     and          submit  this                  file</strong></td>

   <td width="433">Implementation  file            for            <strong>Rectangle</strong>              class</td>

  </tr>

  <tr>

   <td width="110"><strong>color.h  </strong></td>

   <td width="191">Included</td>

   <td width="433">Specification         file            for            <strong>Color</strong>      class</td>

  </tr>

  <tr>

   <td width="110"><strong>color.cpp</strong><strong>                  </strong></td>

   <td width="191"><strong>Write     and          submit  this                  file</strong></td>

   <td width="433">Implementation  file            for            <strong>Color</strong>      class</td>

  </tr>

  <tr>

   <td width="110"><strong>p02input1.txt                  </strong></td>

   <td width="191">Included</td>

   <td width="433">Tests       class        <strong>Shape</strong>    member                  functions</td>

  </tr>

  <tr>

   <td width="110"><strong>p02input2.txt</strong><strong>                  </strong></td>

   <td width="191">Included</td>

   <td width="433">Tests       class        <strong>Triangle</strong>                 member                  functions</td>

  </tr>

  <tr>

   <td width="110"><strong>p02input3.txt</strong><strong>                  </strong></td>

   <td width="191">Included</td>

   <td width="433">Tests       class        <strong>Rectangle</strong>              member                  functions</td>

  </tr>

 </tbody>

</table>




<h1>Step #1 – Unzipping Project Materials on blackhawk</h1>

Use      the      Firefox            browser          to         access Canvas            and      download       the      <strong>Project02_Materials.zip</strong>     file       into your    <strong>Project02</strong>      directory.                   At        terminal         window          prompt,          use      the      unzip  utility  to uncompress   the      files.                For      example,         to         unzip  the      files     into     your    current           directory:

<strong>unzip  Project02_Materials.zip </strong>

Since   this      project            is         worth  three   points, you      have    been    given   three   input   files     to         test      your    program.

<h1>Step #2 – Create Function Stubs for the Missing Support Functions</h1>

Open   a          Linux  terminal         window          and      navigate         to         the      directory        containing      the      <strong>Project02</strong> materials        downloaded   from    Canvas            (you    should be        there   already           if          you      just      completed      Step    #1 above).

Use      the      following        command       to         create the      missing           files     by        typing the      following        at         the Linux  prompt.                      Linux  is         case     sensitive         so        pay      attention        to         upper  versus lower  case     letters.

<h2>gedit color.cpp shape.h triangle.cpp rectangle.cpp &amp;</h2>

This     command       starts  the      <strong>gedit</strong>   text     editor  running          as        a          background    process           (          <strong>&amp;</strong>         ).          With    the      editor  running          in         the      background,   you      may     use      the      same   terminal         window          to compile          and      test      your    program.

—          Place   the      missing           <strong>Shape</strong> class    declaration     in         <strong>shape.h</strong><strong>          </strong>

—          Place   stubs   for       <strong>Color</strong>, <strong>Triangle</strong>        and      <strong>Rectangle</strong>      functions        in         <strong>color.cpp</strong>,      <strong>triangle.cpp</strong><strong>  </strong>and <strong>rectangle.cpp</strong><strong>           </strong>and      save    the      files.

In         the      terminal         window,         compile          your    program         by        typing the      word   <strong>make</strong>  at         the      prompt and      press   the      Enter   key.                 If         you      see      error   messages,       use      the      text     editor  to         make   corrections to         the      function          stubs   and      switch back    to         the      terminal         window          to         type    <strong>make</strong>  again   to recompile       your    program.                    Once   your    program         compiles,        you      may     execute           it          by        typing:                                                             <strong>./project02   inputfilename</strong><strong>       </strong>

Now    that     your    program         compiles         and      executes         using   function          stubs,  you      may     implement     and      test your    solution          function          by        function.                     Start    with    the      functions        associated      with    opening          files and      loading           data.

<strong>Running the Sample Solution on blackhawk [shows the desired output for specified input file] </strong><strong><em>The    best     description    of what   your    code    should            do        is         the      Sample           Solution         for       the      project.</em></strong>

Run     the      sample            solution          by        typing the      following        at         <strong>blackhawk</strong>    terminal         window          command prompt           where <strong>inputfilename</strong>     is         the      name   of         one      of         the      provided        input   files     (for     example, p02input1.txt).

<strong>/home/work/cpe212/project02/p02   inputfilename </strong>

Your    current           working          directory        must   contain           the      input   files     for       this      to         work.

<h1>Running the Preview Script on blackhawk [analyzes outputs for all provided input files]</h1>

Run     the      preview          script  by        typing the      following        in         a          <strong>blackhawk</strong>    terminal         window          command prompt

<strong>/home/work/cpe212data/project02/preview02.bash         </strong>

This     script  will      run      both    the      <strong>Sample           Solution</strong>         AND    your    <strong>project02</strong>      executable      program         on        the complete        set       of         input   files,    and      it          compares       the      outputs           of         the      two     programs       line      by line      to         identify           errors in         your    program’s      outputs.                      Make   sure    that     the      output of         your program         exactly            matches          the      output of         the      Sample           Solution.

<ul>

 <li><strong><em>To use      the      preview          script, your    executable     must   be        on       </em></strong><strong><em>blackhawk</em></strong><strong><em>    </em></strong></li>

 <li><strong><em>The sample           input  files     must   be        in        your    current          working         directory       BEFORE          you execute          the      preview          script!!!          </em></strong></li>

</ul>


