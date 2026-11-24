O arquivo original deve permanecer exatamente como foi fornecido. O código revisado fica em outro arquivo, na pasta revisado.
2. Excel — análise estática
A aba CAIXA BRANCA (ESTÁTICO) está preenchida com os oito itens revisados:
ID	Item	Status
1	Documentação do código	NÃO
2	Nomenclatura de arquivos e classes	SIM
3	Nomenclatura de variáveis e constantes	SIM
4	Loop sem condição de parada	NÃO
5	NullPointer não tratado	NÃO
6	Variável não inicializada	NÃO
7	Arquitetura e separação de responsabilidades	NÃO
8	Tratamento de exceções	NÃO

Os status se referem à presença dos problemas descritos na análise. Nos itens 4, 5 e 6, por exemplo, NÃO significa que não foi identificado o problema perguntado.

Falta conferir: os campos Projeto/Sistema, Revisor e Data da Revisão no cabeçalho. Não precisa refazer os oito itens.
3. Grafos e complexidade ciclomática
Método consultarQuantidade(String codigo)
Use o grafo abaixo e salve seu código Mermaid em diagramas/consultarQuantidade.mmd.
#chatgpt-mermaid-_r_1pa_{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:16px;fill:rgb(13, 13, 13);}@keyframes edge-animation-frame{from{stroke-dashoffset:0;}}@keyframes dash{to{stroke-dashoffset:0;}}#chatgpt-mermaid-_r_1pa_ .edge-animation-slow{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 50s linear infinite;stroke-linecap:round;}#chatgpt-mermaid-_r_1pa_ .edge-animation-fast{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 20s linear infinite;stroke-linecap:round;}#chatgpt-mermaid-_r_1pa_ .error-icon{fill:rgb(243, 243, 243);}#chatgpt-mermaid-_r_1pa_ .error-text{fill:rgb(13, 13, 13);stroke:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pa_ .edge-thickness-normal{stroke-width:1px;}#chatgpt-mermaid-_r_1pa_ .edge-thickness-thick{stroke-width:3.5px;}#chatgpt-mermaid-_r_1pa_ .edge-pattern-solid{stroke-dasharray:0;}#chatgpt-mermaid-_r_1pa_ .edge-thickness-invisible{stroke-width:0;fill:none;}#chatgpt-mermaid-_r_1pa_ .edge-pattern-dashed{stroke-dasharray:3;}#chatgpt-mermaid-_r_1pa_ .edge-pattern-dotted{stroke-dasharray:2;}#chatgpt-mermaid-_r_1pa_ .marker{fill:rgb(143, 143, 143);stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pa_ .marker.cross{stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pa_ svg{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:16px;}#chatgpt-mermaid-_r_1pa_ p{margin:0;}#chatgpt-mermaid-_r_1pa_ .label{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pa_ .cluster-label text{fill:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pa_ .cluster-label span{color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pa_ .cluster-label span p{background-color:transparent;}#chatgpt-mermaid-_r_1pa_ .label text,#chatgpt-mermaid-_r_1pa_ span{fill:rgb(13, 13, 13);color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pa_ .node rect,#chatgpt-mermaid-_r_1pa_ .node circle,#chatgpt-mermaid-_r_1pa_ .node ellipse,#chatgpt-mermaid-_r_1pa_ .node polygon,#chatgpt-mermaid-_r_1pa_ .node path{fill:rgb(222, 234, 251);stroke:rgb(83, 154, 248);stroke-width:1px;}#chatgpt-mermaid-_r_1pa_ .rough-node .label text,#chatgpt-mermaid-_r_1pa_ .node .label text,#chatgpt-mermaid-_r_1pa_ .image-shape .label,#chatgpt-mermaid-_r_1pa_ .icon-shape .label{text-anchor:middle;}#chatgpt-mermaid-_r_1pa_ .node .katex path{fill:#000;stroke:#000;stroke-width:1px;}#chatgpt-mermaid-_r_1pa_ .rough-node .label,#chatgpt-mermaid-_r_1pa_ .node .label,#chatgpt-mermaid-_r_1pa_ .image-shape .label,#chatgpt-mermaid-_r_1pa_ .icon-shape .label{text-align:center;}#chatgpt-mermaid-_r_1pa_ .node.clickable{cursor:pointer;}#chatgpt-mermaid-_r_1pa_ .root .anchor path{fill:rgb(143, 143, 143)!important;stroke-width:0;stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pa_ .arrowheadPath{fill:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pa_ .edgePath .path{stroke:rgb(143, 143, 143);stroke-width:1px;}#chatgpt-mermaid-_r_1pa_ .flowchart-link{stroke:rgb(143, 143, 143);fill:none;}#chatgpt-mermaid-_r_1pa_ .edgeLabel{background-color:rgb(252, 252, 252);text-align:center;}#chatgpt-mermaid-_r_1pa_ .edgeLabel p{background-color:rgb(252, 252, 252);}#chatgpt-mermaid-_r_1pa_ .edgeLabel rect{opacity:0.5;background-color:rgb(252, 252, 252);fill:rgb(252, 252, 252);}#chatgpt-mermaid-_r_1pa_ .labelBkg{background-color:rgba(252, 252, 252, 0.5);}#chatgpt-mermaid-_r_1pa_ .cluster rect{fill:rgb(243, 243, 243);stroke:rgba(0, 0, 0, 0.1);stroke-width:1px;}#chatgpt-mermaid-_r_1pa_ .cluster text{fill:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pa_ .cluster span{color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pa_ div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:12px;background:rgb(243, 243, 243);border:1px solid rgba(0, 0, 0, 0.1);border-radius:2px;pointer-events:none;z-index:100;}#chatgpt-mermaid-_r_1pa_ .flowchartTitleText{text-anchor:middle;font-size:18px;fill:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pa_ rect.text{fill:none;stroke-width:0;}#chatgpt-mermaid-_r_1pa_ .icon-shape,#chatgpt-mermaid-_r_1pa_ .image-shape{background-color:rgb(252, 252, 252);text-align:center;}#chatgpt-mermaid-_r_1pa_ .icon-shape p,#chatgpt-mermaid-_r_1pa_ .image-shape p{background-color:rgb(252, 252, 252);padding:2px;}#chatgpt-mermaid-_r_1pa_ .icon-shape .label rect,#chatgpt-mermaid-_r_1pa_ .image-shape .label rect{opacity:0.5;background-color:rgb(252, 252, 252);fill:rgb(252, 252, 252);}#chatgpt-mermaid-_r_1pa_ .label-icon{display:inline-block;height:1em;overflow:visible;vertical-align:-0.125em;}#chatgpt-mermaid-_r_1pa_ .node .label-icon path{fill:currentColor;stroke:revert;stroke-width:revert;}#chatgpt-mermaid-_r_1pa_ .node .neo-node{stroke:rgb(83, 154, 248);}#chatgpt-mermaid-_r_1pa_ [data-look="neo"].node rect,#chatgpt-mermaid-_r_1pa_ [data-look="neo"].cluster rect,#chatgpt-mermaid-_r_1pa_ [data-look="neo"].node polygon{stroke:url(#chatgpt-mermaid-_r_1pa_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pa_ [data-look="neo"].swimlane.cluster rect{filter:none;}#chatgpt-mermaid-_r_1pa_ [data-look="neo"].node path{stroke:url(#chatgpt-mermaid-_r_1pa_-gradient);stroke-width:1px;}#chatgpt-mermaid-_r_1pa_ [data-look="neo"].node .outer-path{filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pa_ [data-look="neo"].node .neo-line path{stroke:rgb(83, 154, 248);filter:none;}#chatgpt-mermaid-_r_1pa_ [data-look="neo"].node circle{stroke:url(#chatgpt-mermaid-_r_1pa_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pa_ [data-look="neo"].node circle .state-start{fill:#000000;}#chatgpt-mermaid-_r_1pa_ [data-look="neo"].icon-shape .icon{fill:url(#chatgpt-mermaid-_r_1pa_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pa_ [data-look="neo"].icon-shape .icon-neo path{stroke:url(#chatgpt-mermaid-_r_1pa_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pa_ .node text{font-size:14px;font-weight:600;letter-spacing:normal;fill:rgb(0, 79, 153);}#chatgpt-mermaid-_r_1pa_ .edgeLabels text{font-size:13px;font-weight:600;letter-spacing:-0.08px;fill:rgb(0, 79, 153);}#chatgpt-mermaid-_r_1pa_ .node tspan[font-weight="normal"],#chatgpt-mermaid-_r_1pa_ .edgeLabels tspan[font-weight="normal"]{font-weight:600;}#chatgpt-mermaid-_r_1pa_ .edgeLabel .label rect{opacity:1;rx:13px;ry:13px;fill:rgb(245, 250, 255);stroke:rgb(206, 219, 229);stroke-width:1px;}#chatgpt-mermaid-_r_1pa_ .node rect,#chatgpt-mermaid-_r_1pa_ .node circle,#chatgpt-mermaid-_r_1pa_ .node ellipse,#chatgpt-mermaid-_r_1pa_ .node polygon,#chatgpt-mermaid-_r_1pa_ .node path{fill:rgb(229, 243, 255);stroke:rgba(0, 0, 0, 0.1);stroke-width:1px;}#chatgpt-mermaid-_r_1pa_ .node rect{rx:16px;ry:16px;}#chatgpt-mermaid-_r_1pa_ .mermaid-decision .label-container{fill:rgb(245, 250, 255);stroke:rgb(206, 219, 229);stroke-dasharray:2,2;}#chatgpt-mermaid-_r_1pa_ .edgePaths .flowchart-link{stroke:rgb(143, 143, 143);stroke-width:1px;stroke-linecap:round;stroke-linejoin:round;}#chatgpt-mermaid-_r_1pa_ .marker{fill:rgb(143, 143, 143);stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pa_ :root{--mermaid-font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";}1. Início e quantidade = 02. Abrir arquivo e testar while3. Separar colunas7. Retornar quantidade6. Catch4. Código encontrado?5. Converter quantidade ebreak8. FimLinha existeFim do arquivoIOExceptionSimNão





Contagem adotada:
- Nós: \(N=8\)
- Arestas: \(E=10\)
- Componentes conectados: \(P=1\)
\[
V(G)=E-N+2P=10-8+2=\boxed{4}
\]

Caminhos independentes:
Caminho	Sequência de nós	Descrição
P1	1 → 2 → 6 → 7 → 8	Ocorre IOException.
P2	1 → 2 → 7 → 8	Arquivo vazio.
P3	1 → 2 → 3 → 4 → 2 → 7 → 8	Código não encontrado após leitura das linhas.
P4	1 → 2 → 3 → 4 → 5 → 7 → 8	Código encontrado e quantidade convertida.

Método registrarSaida(String codigo, int quantidade)
Salve este grafo em diagramas/registrarSaida.mmd.
#chatgpt-mermaid-_r_1pb_{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:16px;fill:rgb(13, 13, 13);}@keyframes edge-animation-frame{from{stroke-dashoffset:0;}}@keyframes dash{to{stroke-dashoffset:0;}}#chatgpt-mermaid-_r_1pb_ .edge-animation-slow{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 50s linear infinite;stroke-linecap:round;}#chatgpt-mermaid-_r_1pb_ .edge-animation-fast{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 20s linear infinite;stroke-linecap:round;}#chatgpt-mermaid-_r_1pb_ .error-icon{fill:rgb(243, 243, 243);}#chatgpt-mermaid-_r_1pb_ .error-text{fill:rgb(13, 13, 13);stroke:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pb_ .edge-thickness-normal{stroke-width:1px;}#chatgpt-mermaid-_r_1pb_ .edge-thickness-thick{stroke-width:3.5px;}#chatgpt-mermaid-_r_1pb_ .edge-pattern-solid{stroke-dasharray:0;}#chatgpt-mermaid-_r_1pb_ .edge-thickness-invisible{stroke-width:0;fill:none;}#chatgpt-mermaid-_r_1pb_ .edge-pattern-dashed{stroke-dasharray:3;}#chatgpt-mermaid-_r_1pb_ .edge-pattern-dotted{stroke-dasharray:2;}#chatgpt-mermaid-_r_1pb_ .marker{fill:rgb(143, 143, 143);stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pb_ .marker.cross{stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pb_ svg{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:16px;}#chatgpt-mermaid-_r_1pb_ p{margin:0;}#chatgpt-mermaid-_r_1pb_ .label{font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pb_ .cluster-label text{fill:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pb_ .cluster-label span{color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pb_ .cluster-label span p{background-color:transparent;}#chatgpt-mermaid-_r_1pb_ .label text,#chatgpt-mermaid-_r_1pb_ span{fill:rgb(13, 13, 13);color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pb_ .node rect,#chatgpt-mermaid-_r_1pb_ .node circle,#chatgpt-mermaid-_r_1pb_ .node ellipse,#chatgpt-mermaid-_r_1pb_ .node polygon,#chatgpt-mermaid-_r_1pb_ .node path{fill:rgb(222, 234, 251);stroke:rgb(83, 154, 248);stroke-width:1px;}#chatgpt-mermaid-_r_1pb_ .rough-node .label text,#chatgpt-mermaid-_r_1pb_ .node .label text,#chatgpt-mermaid-_r_1pb_ .image-shape .label,#chatgpt-mermaid-_r_1pb_ .icon-shape .label{text-anchor:middle;}#chatgpt-mermaid-_r_1pb_ .node .katex path{fill:#000;stroke:#000;stroke-width:1px;}#chatgpt-mermaid-_r_1pb_ .rough-node .label,#chatgpt-mermaid-_r_1pb_ .node .label,#chatgpt-mermaid-_r_1pb_ .image-shape .label,#chatgpt-mermaid-_r_1pb_ .icon-shape .label{text-align:center;}#chatgpt-mermaid-_r_1pb_ .node.clickable{cursor:pointer;}#chatgpt-mermaid-_r_1pb_ .root .anchor path{fill:rgb(143, 143, 143)!important;stroke-width:0;stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pb_ .arrowheadPath{fill:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pb_ .edgePath .path{stroke:rgb(143, 143, 143);stroke-width:1px;}#chatgpt-mermaid-_r_1pb_ .flowchart-link{stroke:rgb(143, 143, 143);fill:none;}#chatgpt-mermaid-_r_1pb_ .edgeLabel{background-color:rgb(252, 252, 252);text-align:center;}#chatgpt-mermaid-_r_1pb_ .edgeLabel p{background-color:rgb(252, 252, 252);}#chatgpt-mermaid-_r_1pb_ .edgeLabel rect{opacity:0.5;background-color:rgb(252, 252, 252);fill:rgb(252, 252, 252);}#chatgpt-mermaid-_r_1pb_ .labelBkg{background-color:rgba(252, 252, 252, 0.5);}#chatgpt-mermaid-_r_1pb_ .cluster rect{fill:rgb(243, 243, 243);stroke:rgba(0, 0, 0, 0.1);stroke-width:1px;}#chatgpt-mermaid-_r_1pb_ .cluster text{fill:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pb_ .cluster span{color:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pb_ div.mermaidTooltip{position:absolute;text-align:center;max-width:200px;padding:2px;font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";font-size:12px;background:rgb(243, 243, 243);border:1px solid rgba(0, 0, 0, 0.1);border-radius:2px;pointer-events:none;z-index:100;}#chatgpt-mermaid-_r_1pb_ .flowchartTitleText{text-anchor:middle;font-size:18px;fill:rgb(13, 13, 13);}#chatgpt-mermaid-_r_1pb_ rect.text{fill:none;stroke-width:0;}#chatgpt-mermaid-_r_1pb_ .icon-shape,#chatgpt-mermaid-_r_1pb_ .image-shape{background-color:rgb(252, 252, 252);text-align:center;}#chatgpt-mermaid-_r_1pb_ .icon-shape p,#chatgpt-mermaid-_r_1pb_ .image-shape p{background-color:rgb(252, 252, 252);padding:2px;}#chatgpt-mermaid-_r_1pb_ .icon-shape .label rect,#chatgpt-mermaid-_r_1pb_ .image-shape .label rect{opacity:0.5;background-color:rgb(252, 252, 252);fill:rgb(252, 252, 252);}#chatgpt-mermaid-_r_1pb_ .label-icon{display:inline-block;height:1em;overflow:visible;vertical-align:-0.125em;}#chatgpt-mermaid-_r_1pb_ .node .label-icon path{fill:currentColor;stroke:revert;stroke-width:revert;}#chatgpt-mermaid-_r_1pb_ .node .neo-node{stroke:rgb(83, 154, 248);}#chatgpt-mermaid-_r_1pb_ [data-look="neo"].node rect,#chatgpt-mermaid-_r_1pb_ [data-look="neo"].cluster rect,#chatgpt-mermaid-_r_1pb_ [data-look="neo"].node polygon{stroke:url(#chatgpt-mermaid-_r_1pb_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pb_ [data-look="neo"].swimlane.cluster rect{filter:none;}#chatgpt-mermaid-_r_1pb_ [data-look="neo"].node path{stroke:url(#chatgpt-mermaid-_r_1pb_-gradient);stroke-width:1px;}#chatgpt-mermaid-_r_1pb_ [data-look="neo"].node .outer-path{filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pb_ [data-look="neo"].node .neo-line path{stroke:rgb(83, 154, 248);filter:none;}#chatgpt-mermaid-_r_1pb_ [data-look="neo"].node circle{stroke:url(#chatgpt-mermaid-_r_1pb_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pb_ [data-look="neo"].node circle .state-start{fill:#000000;}#chatgpt-mermaid-_r_1pb_ [data-look="neo"].icon-shape .icon{fill:url(#chatgpt-mermaid-_r_1pb_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pb_ [data-look="neo"].icon-shape .icon-neo path{stroke:url(#chatgpt-mermaid-_r_1pb_-gradient);filter:drop-shadow( 1px 2px 2px rgba(185,185,185,1));}#chatgpt-mermaid-_r_1pb_ .node text{font-size:14px;font-weight:600;letter-spacing:normal;fill:rgb(0, 79, 153);}#chatgpt-mermaid-_r_1pb_ .edgeLabels text{font-size:13px;font-weight:600;letter-spacing:-0.08px;fill:rgb(0, 79, 153);}#chatgpt-mermaid-_r_1pb_ .node tspan[font-weight="normal"],#chatgpt-mermaid-_r_1pb_ .edgeLabels tspan[font-weight="normal"]{font-weight:600;}#chatgpt-mermaid-_r_1pb_ .edgeLabel .label rect{opacity:1;rx:13px;ry:13px;fill:rgb(245, 250, 255);stroke:rgb(206, 219, 229);stroke-width:1px;}#chatgpt-mermaid-_r_1pb_ .node rect,#chatgpt-mermaid-_r_1pb_ .node circle,#chatgpt-mermaid-_r_1pb_ .node ellipse,#chatgpt-mermaid-_r_1pb_ .node polygon,#chatgpt-mermaid-_r_1pb_ .node path{fill:rgb(229, 243, 255);stroke:rgba(0, 0, 0, 0.1);stroke-width:1px;}#chatgpt-mermaid-_r_1pb_ .node rect{rx:16px;ry:16px;}#chatgpt-mermaid-_r_1pb_ .mermaid-decision .label-container{fill:rgb(245, 250, 255);stroke:rgb(206, 219, 229);stroke-dasharray:2,2;}#chatgpt-mermaid-_r_1pb_ .edgePaths .flowchart-link{stroke:rgb(143, 143, 143);stroke-width:1px;stroke-linecap:round;stroke-linejoin:round;}#chatgpt-mermaid-_r_1pb_ .marker{fill:rgb(143, 143, 143);stroke:rgb(143, 143, 143);}#chatgpt-mermaid-_r_1pb_ :root{--mermaid-font-family:-apple-system-body,ui-sans-serif,-apple-system,system-ui,"Segoe UI",Helvetica,"Apple Color Emoji",Arial,sans-serif,"Segoe UI Emoji","Segoe UI Symbol";}1. Início e consulta ao estoque2. Quantidade <= disponível?6. Retornar false3. Abrir arquivo e gravarmovimentação5. Atualizar últimamovimentação e retornar true4. Catch7. FimNãoSimSucessoIOException





Contagem adotada:
- Nós: \(N=7\)
- Arestas: \(E=8\)
- Componentes conectados: \(P=1\)
\[
V(G)=E-N+2P=8-7+2=\boxed{3}
\]

Caminhos independentes:
Caminho	Sequência de nós	Descrição
P1	1 → 2 → 6 → 7	Quantidade maior que o estoque.
P2	1 → 2 → 3 → 5 → 7	Gravação concluída.
P3	1 → 2 → 3 → 4 → 6 → 7	Ocorre IOException durante a gravação.

Esses cálculos correspondem à convenção dos grafos acima, incluindo o caminho excepcional. Mantenha a mesma numeração nos diagramas e no relatório.





4. Código original
Salve o código original que você enviou em original/EstoqueArquivo.java, sem modificações:
  import java.io.BufferedReader;
import java.io.FileReader;
import java.io.FileWriter;
import java.io.IOException;

/** Código-base intencionalmente problemático para revisão estática e estrutural. */
public class EstoqueArquivo {
    private String ultimaMovimentacao = "";

    public int consultarQuantidade(String codigo) {
        int quantidade = 0;
        try {
            BufferedReader leitor = new BufferedReader(
                    new FileReader("estoque.csv"));
            String linha;

            while ((linha = leitor.readLine()) != null) {
                String[] colunas = linha.split(";");

                if (colunas[0].equals(codigo)) {
                    quantidade = Integer.parseInt(colunas[1]);
                    break;
                }
            }
        } catch (IOException e) {
            // Erro de leitura ignorado.
        }

        return quantidade;
    }

    public boolean registrarSaida(String codigo, int quantidade) {
        int disponivel = consultarQuantidade(codigo);

        if (quantidade <= disponivel) {
            try {
                FileWriter escrita =
                        new FileWriter("movimentacoes.txt", true);

                escrita.write(codigo + ";" + quantidade + "\n");
                ultimaMovimentacao = codigo;
                return true;
            } catch (IOException e) {
                // Falha ignorada.
            }
        }

        return false;
    }

    public String getUltimaMovimentacao() {
        return ultimaMovimentacao;
    }
}

--5. Código revisado
Salve em revisado/EstoqueArquivo.java. Esta versão valida entradas, fecha os arquivos automaticamente e comunica falhas por exceções.

import java.io.BufferedReader;
import java.io.BufferedWriter;
import java.io.IOException;
import java.nio.file.Files;
import java.nio.file.Path;
import java.nio.file.StandardOpenOption;

public class EstoqueArquivo {
    private static final Path ARQUIVO_ESTOQUE =
            Path.of("estoque.csv");

    private static final Path ARQUIVO_MOVIMENTACOES =
            Path.of("movimentacoes.txt");

    private String ultimaMovimentacao = "";

    public int consultarQuantidade(String codigo) {
        validarCodigo(codigo);

        try (BufferedReader leitor =
                     Files.newBufferedReader(ARQUIVO_ESTOQUE)) {

            String linha;

            while ((linha = leitor.readLine()) != null) {
                String[] colunas = linha.split(";", -1);

                if (colunas.length != 2) {
                    throw new IllegalStateException(
                            "Linha inválida no arquivo de estoque.");
                }

                if (colunas[0].equals(codigo)) {
                    try {
                        return Integer.parseInt(colunas[1]);
                    } catch (NumberFormatException e) {
                        throw new IllegalStateException(
                                "Quantidade inválida no arquivo.", e);
                    }
                }
            }

            return 0;

        } catch (IOException e) {
            throw new IllegalStateException(
                    "Não foi possível ler o arquivo de estoque.", e);
        }
    }

    public boolean registrarSaida(String codigo, int quantidade) {
        validarCodigo(codigo);

        if (quantidade <= 0) {
            throw new IllegalArgumentException(
                    "A quantidade deve ser maior que zero.");
        }

        int disponivel = consultarQuantidade(codigo);

        if (quantidade > disponivel) {
            return false;
        }

        try (BufferedWriter escrita = Files.newBufferedWriter(
                ARQUIVO_MOVIMENTACOES,
                StandardOpenOption.CREATE,
                StandardOpenOption.APPEND)) {

            escrita.write(codigo + ";" + quantidade);
            escrita.newLine();

            ultimaMovimentacao = codigo;
            return true;

        } catch (IOException e) {
            throw new IllegalStateException(
                    "Não foi possível registrar a movimentação.", e);
        }
    }

    public String getUltimaMovimentacao() {
        return ultimaMovimentacao;
    }

    private void validarCodigo(String codigo) {
        if (codigo == null || codigo.isBlank()) {
            throw new IllegalArgumentException(
                    "O código não pode ser nulo ou vazio.");
        }
    }
}

Limitação conhecida: essa versão ainda registra a saída em movimentacoes.txt, mas não reduz a quantidade armazenada em estoque.csv. Se o requisito funcional exigir que o estoque seja atualizado, será necessário implementar essa regra e incluir testes próprios. Não apresente essa funcionalidade como concluída.
6. Plano de testes
Salve a matriz em testes/PlanoDeTestes.md e registre os resultados efetivamente observados.
ID	Método	Cenário	Entrada e pré-condição	Resultado esperado no original
T01	consultarQuantidade	Código existente	CSV contém ABC;10	Retorna 10
T02	consultarQuantidade	Arquivo vazio	CSV vazio	Retorna 0
T03	consultarQuantidade	Código inexistente	CSV contém outro código válido	Retorna 0
T04	consultarQuantidade	Arquivo inexistente	CSV indisponível	Retorna 0, pois a IOException é ignorada
T05	registrarSaida	Saída válida	CSV contém ABC;10; saída 3	Retorna true e grava a movimentação
T06	registrarSaida	Estoque insuficiente	CSV contém ABC;10; saída 11	Retorna false
T07	registrarSaida	Quantidade igual ao estoque	CSV contém ABC;10; saída 10	Retorna true
T08	registrarSaida	Falha de gravação	Estoque suficiente; destino não gravável	Retorna false se ocorrer IOException
T09	registrarSaida	Quantidade negativa	CSV contém ABC;10; saída -2	O original aceita a condição e pode gravar a quantidade negativa
T10	consultarQuantidade	CSV malformado	Campo ausente ou quantidade não numérica	Pode lançar exceção não tratada

Comparação com o código revisado
ID	Resultado esperado no revisado
T01	Retorna 10
T02	Retorna 0
T03	Retorna 0
T04	Lança IllegalStateException por falha na leitura
T05	Retorna true e grava a movimentação
T06	Retorna false
T07	Retorna true
T08	Lança IllegalStateException se ocorrer falha de gravação
T09	Lança IllegalArgumentException
T10	Lança IllegalStateException para a linha inválida ou quantidade não numérica encontrada

Para T08, a falha precisa ser provocada e confirmada no ambiente usado. Não presuma que um arquivo inacessível produzirá o mesmo resultado em todos os sistemas.
7. Classe de teste manual
Salve em testes/TesteEstoque.java. Ela permite iniciar a execução, mas não substitui os dez cenários da matriz.


public class TesteEstoque {
    public static void main(String[] args) {
        EstoqueArquivo estoque = new EstoqueArquivo();

        try {
            int quantidade =
                    estoque.consultarQuantidade("ABC");

            System.out.println(
                    "Quantidade encontrada: " + quantidade);

            boolean resultado =
                    estoque.registrarSaida("ABC", 3);

            System.out.println(
                    "Saída registrada: " + resultado);

            System.out.println(
                    "Última movimentação: "
                    + estoque.getUltimaMovimentacao());

        } catch (RuntimeException e) {
            System.err.println(
                    "Falha durante o teste: " + e.getMessage());
        }
    }
}

Prepare o arquivo estoque.csv na pasta de execução:
ABC;10
XYZ;5


Execute o código original e o revisado separadamente. Não reutilize uma pasta com arquivos alterados sem verificar seu conteúdo, porque isso pode interferir nos resultados.





8. README.md completo
Salve o texto abaixo em README.md. Ele documenta a atividade sem afirmar que os testes já foram executados.

# Teste de Caixa Branca e Revisão de Código-Fonte

## Introdução

Este projeto apresenta a análise estática e estrutural de uma aplicação Java que consulta quantidades de produtos em um arquivo CSV e registra movimentações de saída em um arquivo de texto. A atividade utiliza técnicas de teste de caixa branca para avaliar o fluxo de controle, a complexidade ciclomática e os caminhos independentes dos métodos analisados.

## Objetivo da Atividade

Analisar o código original, identificar problemas de qualidade, construir os grafos de fluxo de controle, calcular a complexidade ciclomática, elaborar casos de teste, revisar o código e comparar as duas versões.

## Configuração do Ambiente

A execução requer um JDK compatível com os recursos utilizados no código revisado, incluindo `Path.of` e `String.isBlank`. Recomenda-se Java 11 ou superior.

A aplicação utiliza os arquivos locais `estoque.csv` e `movimentacoes.txt`. O arquivo CSV deve conter o código do produto e sua quantidade, separados por ponto e vírgula.

## Análise Estática

A análise identificou ausência de documentação detalhada, possibilidade de leitura de linhas malformadas, tratamento insuficiente de exceções, falta de validação de entradas e ausência de fechamento explícito de recursos no código original.

Também foi identificada a concentração de leitura do estoque, regra de consulta e gravação de movimentações na mesma classe.

## Grafos e Complexidade Ciclomática

O método `consultarQuantidade(String codigo)` apresenta complexidade ciclomática estimada em 4, conforme o grafo elaborado, incluindo o caminho de `IOException`.

O método `registrarSaida(String codigo, int quantidade)` apresenta complexidade ciclomática estimada em 3, conforme o grafo elaborado, incluindo o caminho de `IOException`.

Os caminhos independentes foram definidos a partir dos grafos registrados na pasta `diagramas`.

## Código Revisado

A versão revisada utiliza validação de código e quantidade, `try-with-resources` para fechamento automático dos arquivos e tratamento explícito de falhas de leitura, conversão e gravação.

A versão apresentada ainda não atualiza o arquivo de estoque após registrar uma saída. Essa limitação deve ser considerada na avaliação dos requisitos funcionais.

## Plano de Testes

O plano contempla dez cenários relacionados à consulta de estoque, códigos existentes e inexistentes, arquivo vazio, falhas de leitura e gravação, estoque insuficiente, quantidade negativa e linhas malformadas.

Os resultados esperados são definidos separadamente para o código original e o revisado, pois a versão revisada trata determinadas falhas por meio de exceções.

## Execução e Registro dos Testes

Os testes devem ser executados individualmente nas duas versões. Para cada cenário, devem ser registrados o resultado obtido, o status de aprovação ou reprovação e a evidência correspondente.

Os resultados desta seção devem ser atualizados após a execução real. Não são considerados resultados comprovados aqueles que foram apenas previstos.

## Resultados Obtidos

A análise estrutural estabeleceu os valores de complexidade ciclomática dos dois métodos com base nos grafos apresentados.

A comparação prática entre as versões depende da execução dos casos de teste. Os resultados observados, as diferenças de comportamento e as evidências devem ser acrescentados após essa etapa.

## Conclusão

A atividade permite examinar o fluxo de controle e identificar oportunidades de melhoria na qualidade do código Java. A versão revisada melhora a validação das entradas, o gerenciamento de recursos e a comunicação de falhas.

A conclusão definitiva deve considerar os resultados efetivamente observados, as evidências reunidas e a verificação dos requisitos funcionais do sistema.

