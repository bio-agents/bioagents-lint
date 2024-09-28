# What is bioagentsLint?

**bioagentsLint is under design : coding has not started and this page may be missing information**

**bioagentsLint** is a utility for verification and reporting of content of the [IECHOR Agents & Data Services Registry](https://bio.agents).  It will, for purposes of content quality control and labelling, verify the content according to:
* agent description syntax defined by [bioagents schema](https://github.com/bio-agents/bioagents schema)
* correct or recommended use of the [EDAM ontology](https://github.com/edamontology/edamontology/)
* curation best practice from the bio.agents [Curators Guide](https://bioagents.readthedocs.io/en/latest/curators_guide.html) (in so far as these recommendations can be automatically verified)
* compliance to the [Agent Information Standard](https://bio-agents.github.io/Agent-Information-Standard/)
* miscellaneous other checks, *e.g.* broken link detection, agent name uniqueness *etc.* 


## Verifications 

The verifications are exhaustively tabulated below, including one table / element group defined in bioagents schema.

### Element-specific verifications

![summary group](images/agent.png)


- [Summary group](https://github.com/bio-agents/bioagentslint#summary-group)
- [Function group](https://github.com/bio-agents/bioagentslint#function-group)
- [Labels group](https://github.com/bio-agents/bioagentslint#labels-group)
- [Links group](https://github.com/bio-agents/bioagentslint#links-group)
- [Download group](https://github.com/bio-agents/bioagentslint#download-group)
- [Documentation group](https://github.com/bio-agents/bioagentslint#documentation-group)
- [Publications group](https://github.com/bio-agents/bioagentslint#publications-group)
- [Credits group](https://github.com/bio-agents/bioagentslint#credits-group)


### General verifications

- [Other general verifications](https://github.com/bio-agents/bioagentslint#other-general-verifications)



## Summary group

See <a href=https://bioagents-schema.readthedocs.io/en/latest/bioagents-schema_elements.html#summary-group>schema docs</a> & <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#summary-group>curators guide</a>

![summary group](images/summary.png)

![otherid](images/otherid.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>


<!--- summary->name --->

<tr><td colspan="4"><b>name:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#name>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#name-agent>curators guide</a> </td></tr>
<tr>
    <td>Invalid cardinality (1 only allowed)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/33>33</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Name is taken (not unique within bio.agents)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/30>30<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (disallowed characters)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/37>37<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Includes technical jargon</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/31>31<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Includes version or status info</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/26>26<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Name similarity (full-length exact match to substring of existing agent name)</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/32>32<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->description --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>description:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#description>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#description>curators guide</a> </td></tr>
<tr>
    <td>Invalid cardinality (1 only allowed)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/33>33</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Wrong or missing capitalisation and full stops</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/35>35<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Includes DOI(s)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/28>28<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Includes URL(s)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/27>27<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->homepage --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>homepage:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#homepage>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#homepage>curators guide</a> </td></tr>
<tr>
    <td>Invalid cardinality (1 only allowed)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/33>33</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Broken link</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/12>12<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Uses existing agent homepage URL</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/38>38<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->bioagentsID --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>bioagentsID:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#bioagentsid>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#summary-bioagentsID>curators guide</a> </td></tr>

<tr>
    <td>Mismatch of bioagentsID & bioagentsCURIE</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/22>22<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->bioagentsCURIE --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>bioagentsCURIE:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#bioagentscurie>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#summary-bioagentscurie>curators guide</a> </td></tr>

<tr>
    <td>Mismatch of bioagentsID & bioagentsCURIE</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/22>22<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->version --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>version:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#version>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#version-agent>curators guide</a> </td></tr>

<tr>
    <td>Invalid syntax (disallowed characters)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/37>37<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>

<!--- summary->otherID --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>otherID:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#other-ids>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#other-ids>curators guide</a> </td></tr>

<tr><td colspan="4"><b>otherID->value</b>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"><b>otherID->type</b>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"><b>otherID->version</b>
<tr>
    <td>Invalid syntax (disallowed characters)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/37>37<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
</table>


## Function group

See <a href=https://bioagents-schema.readthedocs.io/en/latest/bioagents-schema_elements.html#function-group>schema docs</a> & <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#function-group>curators guide</a>

![function group](images/function.png)

![operation](images/operation.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>


<!--- function->operation --->

<tr><td colspan="4"><b>operation:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#operation>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#operation>curators guide</a> </td></tr>

<tr><td colspan="4"><b>operation->uri</b></tr>
<tr>
    <td>Placeholder EDAM concept (not normally used for annotation)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/10>10</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Deprecated EDAM concept</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/6>6</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Duplicated operation</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/3>3</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Undefined Operation::Topic relation</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/41>41</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Missing input</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/42>42</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Missing output</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/43>43</a></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"><b>operation->term</b></tr>
<tr>
    <td>Invalid term</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/7>7</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Use of synonym</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/8>8</a></td>
    <td>tbd</td>
</tr>


<!--- function->input|output->data --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>input|output->data:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#data>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#data-type-input-and-output-data>curators guide</a> </td></tr>

<tr><td colspan="4"><b>input|output->data->uri</b></tr>
<tr>
    <td>Placeholder EDAM concept (not normally used for annotation)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/10>10</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Deprecated EDAM concept</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/6>6</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Undefined Data::Topic relation</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/41>41</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Undefined Data::Operation relation</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/41>41</a></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"><b>data->term</b></tr>
<tr>
    <td>Invalid term</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/7>7</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Use of synonym</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/8>8</a></td>
    <td>tbd</td>
</tr>


<!--- function->input|output->format --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>input|output->format:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#format>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#data-format-input-and-output-data>curators guide</a> </td></tr>

<tr><td colspan="4"><b>input|output->format->uri</b></tr>
<tr>
    <td>Placeholder EDAM concept (not normally used for annotation)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/10>10</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Deprecated EDAM concept</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/6>6</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Duplicated format</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/3>3</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Undefined Data::Format relation</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/41>41</a></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"><b>format->term</b></tr>
<tr>
    <td>Invalid term</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/7>7</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Use of synonym</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/8>8</a></td>
    <td>tbd</td>
</tr>


<!--- function->note --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>note:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#function>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#note-function>curators guide</a> </td></tr>

<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>

<!--- function->cmd --->

<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>cmd:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#function>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#command>curators guide</a> </td></tr>

<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
</table>

See also the [general EDAM verifications](https://github.com/bio-agents/bioagentslint#general-edam-verifications).



## Labels group

See <a href=https://bioagents-schema.readthedocs.io/en/latest/bioagents-schema_elements.html#labels-group>schema docs</a> & <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#labels-group>curators guide</a>

![labels group](images/labels.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>


<!--- labels->agentType --->

<tr><td colspan="4"><b>agentType:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#agentType>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#agent-type>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Duplicated agentType</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/4>4</a></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- labels->topic --->

<tr><td colspan="4"><b>topic:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#topic>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#topic>curators guide</a> </td></tr>

<tr><td colspan="4"><b>topic->uri</b></tr>
<tr>
    <td>Duplicated topic</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/3>3</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Placeholder EDAM concept (not normally used for annotation)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/10>10</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Deprecated EDAM concept</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/6>6</a></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"><b>topic->term</b></tr>
<tr>
    <td>Invalid term</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/7>7</a></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Use of synonym</td>
    <td>INFO</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/8>8</a></td>
    <td>tbd</td>
</tr>


<tr><td colspan="4"></tr>
<!--- labels->operatingSystem --->

<tr><td colspan="4"><b>operatingSystem:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#operatingSystem>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#operating-system>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Duplicated operatingSystem</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/4>4</a></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- labels->language --->

<tr><td colspan="4"><b>language:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#programming-language>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#programming-language>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Duplicated language</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/4>4</a></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- labels->license --->

<tr><td colspan="4"><b>license:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#license>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#license>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- labels->collectionID --->

<tr><td colspan="4"><b>collectionID:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#collection>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#collection>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Duplicated collectionID</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/4>4</a></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- labels->maturity --->

<tr><td colspan="4"><b>maturity:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#maturity>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#maturity>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- labels->cost --->

<tr><td colspan="4"><b>cost:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#cost>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#cost>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- labels->accessibility --->

<tr><td colspan="4"><b>accessibility:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#accessibility>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#accessibility>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Duplicated accessibility</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/4>4</a></td>
    <td>tbd</td>
</tr>
</table>




## Links group

See <a href=https://bioagents-schema.readthedocs.io/en/latest/bioagents-schema_elements.html#links-group>schema docs</a> & <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#links-group>curators guide</a>

![labels group](images/link.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>

<tr><td colspan="4"></tr>
<!--- link->url --->

<tr><td colspan="4"><b>url:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#link>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#url-link>curators guide</a> </td></tr>
<!--- link-url --->
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Broken link</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/12>12<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- link-type --->

<tr><td colspan="4"><b>type:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#link>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#linktype>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- link->note --->

<tr><td colspan="4"><b>note:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#link>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#note-link>curators guide</a> </td></tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
</table>



## Download group

See <a href=https://bioagents-schema.readthedocs.io/en/latest/bioagents-schema_elements.html#download-group>schema docs</a> & <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#download-group>curators guide</a>

![labels group](images/download.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>

<tr><td colspan="4"></tr>
<!--- download->url --->

<tr><td colspan="4"><b>url:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#download>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#url-download>curators guide</a> </td></tr>
<!--- download-url --->
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Broken link/td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/12>12<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- download-type --->

<tr><td colspan="4"><b>type:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#download>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#downloadt-ype>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- download->note --->

<tr><td colspan="4"><b>note:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#download>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#note-download>curators guide</a> </td></tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
</table>



## Documentation group

See <a href=https://bioagents-schema.readthedocs.io/en/latest/bioagents-schema_elements.html#documentation-group>schema docs</a> & <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#documentation-group>curators guide</a>

![labels group](images/documentation.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>

<tr><td colspan="4"></tr>
<!--- documentation->url --->

<tr><td colspan="4"><b>url:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#documentation>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#url-documentation>curators guide</a> </td></tr>
<!--- documentation-url --->
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Broken link</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/12>12<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- documentation-type --->

<tr><td colspan="4"><b>type:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#documentation>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#documentationtype>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- documentation->note --->

<tr><td colspan="4"><b>note:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#documentation>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#note-documentation>curators guide</a> </td></tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
</table>



## Publications group

See <a href=https://bioagents-schema.readthedocs.io/en/latest/bioagents-schema_elements.html#publications-group>schema docs</a> & <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#publications-group>curators guide</a>

![labels group](images/publication.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>

<!--- General publication verifications --->

<tr><td colspan="4"><b>General publication verifications:</b></tr>
<tr>
    <td>Duplicate publication ID</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/2>2<a/>, <a href=https://github.com/bio-agents/bioagentsLint/issues/1>1<a/></td>
    <td>tbd</td>
</tr>


<tr><td colspan="4"></tr>
<!--- publication->doi --->

<tr><td colspan="4"><b>doi:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#publication>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#digital-object-id>curators guide</a> </td></tr>
<!--- publication-doi --->
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Suspect DOI syntax (terminal fullstop)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/23>23<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Unresolvable publication ID</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/5>5<a/>, <a href=https://github.com/bio-agents/bioagentsLint/issues/20>20<a/></td>
    <td>tbd</td>
</tr>


<!--- publication-pmid --->
<tr><td colspan="4"><b>pmid:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#publication>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#pubmed-id>curators guide</a> </td></tr>
<tr><td colspan="4"></tr>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Unresolvable publication ID</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/5>5<a/></td>
    <td>tbd</td>
</tr>


<!--- publication-pmcid --->
<tr><td colspan="4"><b>pmcid:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#publication>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#pubmed-central-id>curators guide</a> </td></tr>
<tr><td colspan="4"></tr>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Unresolvable publication ID</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/5>5<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- publication-type --->

<tr><td colspan="4"><b>type:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#publication>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#publication-type>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- publication->version --->

<tr><td colspan="4"><b>version:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#publication>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#version-publication>curators guide</a> </td></tr>
<tr>
    <td>Invalid syntax (disallowed characters)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/37>37<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
</table>


## Credits group

See <a href=https://bioagents-schema.readthedocs.io/en/latest/bioagents-schema_elements.html#credits-group>schema docs</a> & <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#credits-group>curators guide</a>

![labels group](images/credit.png)

<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>


<!--- General credit verifications --->

<tr><td colspan="4"><b>General credit verifications:</b></tr>
<tr>
    <td>Duplicate credit (of various types)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/14>14<a/></td>
    <td>tbd</td>
</tr>


<tr><td colspan="4"></tr>
<!--- credit->iechorNode --->

<tr><td colspan="4"><b>iechorNode:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#credit>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-iechornode>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Duplicate iechorNode credit</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/13>13<a/></td>
    <td>tbd</td>
</tr>


<tr><td colspan="4"></tr>
<!--- credit->iechorPlatform --->

<tr><td colspan="4"><b>iechorPlatform:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#credit>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#credit-iechorplatform>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Duplicate iechorPlatform credit</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/13>13<a/></td>
    <td>tbd</td>
</tr>


<tr><td colspan="4"></tr>
<!--- credit->name --->

<tr><td colspan="4"><b>name:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#credit>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#name-credit>curators guide</a> </td></tr>
<tr>
    <td>Invalid syntax (disallowed characters)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/37>37<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- credit->email --->

<tr><td colspan="4"><b>email:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#credit>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#email>curators guide</a> </td></tr>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- credit->url --->

<tr><td colspan="4"><b>url:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#credit>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#url-credit>curators guide</a> </td></tr>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Broken link</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/12>12<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- credit->orcidid --->

<tr><td colspan="4"><b>orcidid:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#credit>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#orcid-id>curators guide</a> </td></tr>
<tr>
    <td>Invalid syntax (pattern)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/34>34<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Unresolvable ORCID ID</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/45>45<a/></td>
    <td>tbd</td>
</tr>


<tr><td colspan="4"></tr>
<!--- credit->typeEntity --->

<tr><td colspan="4"><b>typeEntity:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#credit>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#entity-type>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- credit->typeRole --->

<tr><td colspan="4"><b>typeRole:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#credit>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#entity-role>curators guide</a> </td></tr>
<tr>
    <td>Invalid value (must adhere to controlled vocabulary)</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/39>39<a/></td>
    <td>tbd</td>
</tr>

<tr><td colspan="4"></tr>
<!--- credit->note --->

<tr><td colspan="4"><b>note:</b> <a href=https://bioagents.readthedocs.io/en/latest/api_usage_guide.html#credit>API usage</a>, <a href=https://bioagents.readthedocs.io/en/latest/curators_guide.html#note-credit>curators guide</a> </td></tr>
<tr>
    <td>Invalid syntax (disallowed whitespace)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/40>40<a/></td>
    <td>tbd</td>
</tr>
<tr>
    <td>Invalid syntax (length)</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/36>36<a/></td>
    <td>tbd</td>
</tr>
</table>


## General verifications


<table>
<tr>
    <td><b>Verification</b></td>
    <td><b>Log level</b></td>
    <td><b>Issue</b></td>
    <td><b>Status</b></td>
</tr>

<!--- agent IDs --->

<tr><td colspan="4"><b>agent IDs</b> </tr>
<!--- Unverified agentIDs --->
<tr>
    <td>Unverified agentID</td>
    <td>ERROR</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/11>11<a/></td>
    <td>tbd</td>
</tr>

<!--- duplicates --->
<tr><td colspan="4"></tr>
<tr><td colspan="4"><b>duplicates</b> </tr>
<!--- Suspected duplicate entry --->
<tr>
    <td>Suspected duplicate entry</td>
    <td>WARN</td>
    <td><a href=https://github.com/bio-agents/bioagentsLint/issues/25>25<a/></td>
    <td>tbd</td>
</tr>
</table>