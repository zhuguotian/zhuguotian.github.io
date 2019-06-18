## WWW and Internet: same beast, differnt animal
The internet is a global network of networks, the WWW is a collectinos of information which is accessed via the internet. Alternatively, the Internet can be viewed as a big book-store while the Web can be viewed as collection of books on that store. At a high level, we can even think of the Internet as hardware and the Web as software!

## RDF(Resource Description Framework)
RDF is a basic data structure for linked data, and the way data are stored is through triple store. 
>A triple store is designed to store and retrieve identities that are constructed from triplex collections of strings (sequences of letters). These triplex collections represent a subject-predicate-object(主-谓-宾) relationship that more or less corresponds to the definition put forth by the RDF standard.
><p align="right">—Jack Rusher</p>

Here is an example of a RDF data:
'''xml
<?xml version="1.0"?>
<rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
  xmlns:dc="http://purl.org/dc/elements/1.1/">
  <rdf:Description rdf:about="http://www.w3.org/">
    <dc:title>World Wide Web Consortium</dc:title> 
  </rdf:Description>
</rdf:RDF>
'''
By going to w3c RDF verification website, you would have the above code as:
<table frame="border" rules="all">
    <tbody>
        <tr>
            <td>
                <b>Number</b>
            </td>
            <td>
                <b>Subject</b>
            </td>
            <td>
                <b>Predicate</b>
            </td>
            <td>
                <b>Object</b>
            </td>
        </tr>
        <tr>
            <td>1</td>
            <td>
                <a href="http://www.w3.org/">http://www.w3.org/</a>
            </td>
            <td>
                <a href="http://purl.org/dc/elements/1.1/title">http://purl.org/dc/elements/1.1/title</a>
            </td>
            <td>
                "World Wide Web Consortium"
            </td>
        </tr>
    </tbody>
</table>