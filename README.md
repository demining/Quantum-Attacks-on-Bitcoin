

<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/060-2-1024x576.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5302"></figure></div>


<p>Many crypto experts are asking: Will the cryptocurrency industry be able to withstand the new technological revolution? This article will discuss modern methods of protecting financial transactions and the Internet based on cryptography, which may be powerless against a sufficiently powerful quantum computer, and whether cryptocurrencies, whose market is estimated at hundreds of billions of dollars, are vulnerable. The study shows that the proof-of-work algorithm used in Bitcoin is relatively resistant to quantum attacks in the next decade, due to the high speed of specialized mining equipment. However, the elliptic curve digital signature system used by Bitcoin may be hacked by 2027. As an alternative,&nbsp;<a href="https://keyhunters.ru/quantum-resistance-and-momentum-algorithm">the Momentum algorithm</a>&nbsp;is considered , which is more resistant to quantum computing. Other protection methods that can ensure the security and efficiency of blockchain applications in the future are also analyzed.</p>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Overall, the results of the study suggest that quantum computers pose a serious threat to cryptocurrencies, and new security methods need to be developed to ensure their security in the future. We will also use an example to examine the process of compromising the extraction of the secret key Nonce value K from a vulnerable RawTX transaction using the BitcoinChatGPT machine learning process. <sup data-fn="77e87faf-f7a7-4a3c-b1f8-1e4690c475ac" class="fn"><a id="77e87faf-f7a7-4a3c-b1f8-1e4690c475ac-link" href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin-assessing-vulnerabilities-and-developing-defense-strategies-against-emerging-quantum-computing-threats/#77e87faf-f7a7-4a3c-b1f8-1e4690c475ac">1</a></sup></p>
</blockquote>



<p>Bitcoin, as a decentralized and cryptographically protected digital currency, has been successfully in existence since 2008, inspiring the creation of many other cryptocurrencies. Its security is ensured by the proof-of-work mechanism and elliptic curve cryptographic signatures. However, the development of quantum computers poses a serious threat to Bitcoin and all modern cryptography used on the Internet and financial transactions. Research shows that the proof-of-work algorithm used in Bitcoin is relatively resistant to quantum attacks in the next 10 years due to the high speed of specialized mining equipment. But the elliptic curve digital signature system is vulnerable to Shor’s algorithm and could be hacked as early as 2027, allowing attackers to obtain secret keys from Bitcoin transactions and private keys from public ones. Alternative algorithms such as Momentum for proof-of-work and quantum-resistant signature schemes are proposed as a solution. Overall, the findings suggest that quantum computers pose a serious threat to Bitcoin, and new security methods need to be developed to ensure its future security. Quantum computers could&nbsp;<a href="https://keyhunters.ru/quantum-computers-will-hack-bitcoin-in-five-years-opinion/"><em>hack Bitcoin within five years</em></a>&nbsp;. This could&nbsp;<a href="https://polynonce.ru/bitcoins-looming-threat-the-risk-of-quantum-hack/"><em>wipe out more than $3 trillion in cryptocurrency</em></a>&nbsp;and other markets and cause a deep recession.</p>



<p></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p></p>



<p></p>


<div class="wp-block-image">
<figure class="aligncenter size-full"><a href="https://www.youtube.com/watch?v=p62orC7WDUE"><img decoding="async" width="778" height="444" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-9.png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3251" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-9.png 778w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-9-300x171.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-9-768x438.png 768w" sizes="(max-width: 778px) 100vw, 778px"></a></figure></div>


<p></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p></p>



<h3 class="wp-block-heading has-text-align-center">Bitcoin Basics and Attack Protection Principles: Blockchain Mechanism and Proof of Work</h3>



<p></p>



<p>In this part of the article, we will try to explain how Bitcoin works to make it easier to understand possible attacks using quantum computers. The description is given in general terms, since the basic principles of operation are similar to other cryptocurrencies. All transactions are recorded in a public registry – blockchain. Transactions are combined into blocks, which are considered to have occurred simultaneously and are built into a chain. Each block contains a link to the previous one in the form of its hash. New blocks are added by miners using the “proof-of-work” mechanism (Proof-of-Work, PoW). Bitcoin uses the Hashcash algorithm. Miners look for a suitable block header so that its hash is less than a certain value. The header contains information about transactions, the hash of the previous block, a timestamp, and a random number (nonce). The difficulty of the task is selected automatically so that the block is found in about 10 minutes. Bitcoin uses double hashing SHA256.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Python script:&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/DoubleSHA256Hasher.py" target="_blank" rel="noreferrer noopener">DoubleSHA256Hasher.py</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-fa7876f849273a89517e062a3926eb18" style="color:#4092c2"><code><strong>import hashlib

def double_sha256(data):
    """
    Performs double SHA256 hashing on the input data.
    """
    # First pass of SHA256
    hash1 = hashlib.sha256(data).digest()
    # Second pass of SHA256
    hash2 = hashlib.sha256(hash1).digest()
    return hash2

# Example usage
data = b"Example data for double SHA256"  # Data must be represented as bytes
hashed_data = double_sha256(data)
print(hashed_data.hex())  # Output in hexadecimal format
</strong></code></pre>



<p><strong>In this script:</strong></p>



<ol class="wp-block-list">
<li>The module is imported&nbsp;&nbsp;<code><a href="http://grep.cs.msu.ru/python3.8_RU/digitology.tech/docs/python_3/library/hashlib.html">hashlib</a></code>.</li>



<li>A function is defined&nbsp;&nbsp;<code>double_sha256</code> that accepts data in byte format&nbsp;<a href="https://kedu.ru/press-center/articles/info-prog-sekrety-kheshirovaniya-v-python-razberites-s-osnovnymi-metodami/" target="_blank" rel="noreferrer noopener"><sup>2</sup></a>&nbsp;.</li>



<li>Inside the function:
<ul class="wp-block-list">
<li>The SHA256 hash is calculated from the input data using&nbsp;&nbsp;<code>hashlib.sha256(data).digest()</code>. The method&nbsp;&nbsp;<code>.digest()</code>&nbsp;returns the hash as a byte string.</li>



<li>The SHA256 hash is then calculated from the resulting hash.</li>



<li><a href="https://polynonce.ru/python-hashing-secrets-understand-the-basic-methods/">The function returns the second hash</a>&nbsp;.</li>
</ul>
</li>



<li>The usage example shows how to apply the function to a byte string and output the result in&nbsp;<a href="https://polynonce.ru/python-hashing-secrets-understand-the-basic-methods/">hexadecimal format</a>&nbsp;. It is important to note that the input data must be represented in bytes, for this purpose,&nbsp;<code>b"..."</code></li>
</ol>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/Double-SHA-256-accelerator-for-Bitcoin-mining-.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5241"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Miners add the transactions they choose to a block and are rewarded in bitcoins for doing so. When a miner finds a suitable header, they notify the network and the block is added to the blockchain. It is easy to verify the correctness of a PoW solution – you only need to calculate the hash once. PoW is needed to prevent one participant from faking the blockchain, for example, to spend the same money twice. The blockchain can branch, but miners must work on the longest chain. A transaction in Bitcoin is considered confirmed when 6 more blocks are added after it. The article discusses what&nbsp;<a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin">advantage a quantum computer</a>&nbsp;can give when solving PoW and whether it can faking the blockchain. The structure of transactions is also analyzed. When Bob wants to send bitcoins to Alice, Alice creates a pair of keys – private and public. The public key is hashed and the result is an address, which Alice tells Bob. Bitcoin uses the hash of the public key to save space. To send bitcoins, Bob specifies the transactions where he received bitcoins to his addresses. The amount of bitcoins received must be at least as much as the amount Bob wants to send to Alice. Bob proves ownership of the addresses by providing public keys and signing the message with his private key. The choice to use a hash of the public key instead of the key itself affects Bitcoin’s security against quantum attacks.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5141" style="width:840px;height:auto"><figcaption class="wp-element-caption">Illustration of a block. The data at the top makes up the block header.</figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center">Attacks on the Bitcoin Proof-of-Work</h2>



<p>For the most part, a quantum computer can be more efficient than a conventional computer at mining Bitcoin, that is, at performing Proof-of-Work (PoW) based on the hashcash algorithm. A quantum computer using the Grover search algorithm can perform PoW by trying significantly fewer hash options than a classical computer. However, modern ASIC miners, which specialize in calculating hashes, work so fast that this advantage of quantum computers is leveled out, given that the speed of quantum computers is still relatively low. In the future, if the speed of quantum computers can be increased to 100 GHz, they will be able to solve the PoW problem about 100 times faster than now. But this is unlikely to happen in the next 10 years. By that time, both conventional computers will have become faster and quantum technologies will have become more widespread, so no one will be able to single-handedly dominate mining. To assess the security of a blockchain, it is important to understand how much computing power&nbsp;<a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin">a quantum computer would need to successfully solve a PoW problem</a>&nbsp;with a probability greater than 50%. As a result, although quantum computers can theoretically speed up the mining process, in practice, due to the limitations of current technologies, they do not yet pose a serious threat to Bitcoin security. However, in the future, with the development of quantum technologies, this threat may become more real, and it is necessary to develop appropriate security measures to determine how effective a quantum computer can be in mining Bitcoin, taking into account all the technical difficulties and limitations. Grover’s algorithm allows a quantum computer to search for a solution (a suitable block header) much faster than a classical one, but in practice this advantage is greatly reduced.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter size-full"><a href="https://cryptodeeptech.ru/blockchain-attack-vectors/"><img decoding="async" width="835" height="421" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image(1).png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3237" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image.png 835w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-300x151.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-768x387.png 768w" sizes="(max-width: 835px) 100vw, 835px"></a></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>Each hash calculation and block construction requires additional operations, and quantum error correction adds significant overhead. To estimate real-world performance, a model of a universal quantum computer with error correction is used.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-39.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5244"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Calculating the SHA256 hash on a quantum computer requires converting logical operations into reversible quantum operations, which increases the complexity. In addition, quantum computers need to correct errors, which also requires additional resources and time. As a result, the mining speed of a quantum computer depends not only on Grover’s algorithm, but also on many other factors, such as the clock frequency, error rate, complexity of error correction algorithms, and the number of qubits used. The article introduces the concept of “effective hash rate” for a quantum computer (hQC), which takes all these factors into account. The analysis shows that at the current level of technology development, quantum computers are significantly inferior to specialized ASIC miners in hash rate. However, it is expected that in the future, quantum technologies will develop and their performance will increase. The article provides forecasts for the next 25 years and estimates when quantum computers will be able to surpass classical ones in Bitcoin mining. Even if a quantum computer cannot control mining on its own, it could be used to attack mining pools using smart contracts. A small advantage in hashing speed would allow attackers to profit from block manipulation and hold.</p>



<p>Despite the time constraints, the effective hash rate improves asymptotically with the square root of the problem complexity, reflecting the advantage of quantum processors. Grover’s algorithm can be run in parallel on multiple quantum processors. Ideally, each processor searches the entire possible solution space. This reduces the number of oracle queries required to find a solution. As a result, the time to find a solution is reduced and the overall hash rate increases. Grover’s algorithm requires a fixed number of logical qubits (2402), regardless of the complexity of the problem. However, the number of physical qubits required depends on the error correction methods used and is related to the complexity of the problem and the probability of errors.</p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-1.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5144"></figure></div>


<p>The results of the analysis of the performance of quantum computers in attacks on the blockchain are presented&nbsp;<em>in Figure 2.</em>&nbsp;The graph compares the hashing power of the Bitcoin network and one quantum computer over the next 25 years. The estimates are given in optimistic and pessimistic scenarios. According to the optimistic forecast, there will be no quantum computers powerful enough to implement Grover’s algorithm until 2028. For comparison, the graph also shows the hashing speed of modern ASIC devices.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-25-1024x666.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5209"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading">ASIC Device Hash Rate Scheme Description</h2>



<p>Modern ASIC devices for mining cryptocurrencies based on the SHA-256 algorithm (for example, Bitcoin) work as follows:</p>



<ol class="wp-block-list">
<li><strong>Data preprocessing</strong>&nbsp;: Input data is padded to a length that is a multiple of 512 bits.</li>



<li><strong>Initial setup</strong>&nbsp;: Predefined initial hash values ​​are used.</li>



<li><strong>Block processing</strong>&nbsp;: Data is processed in 512-bit blocks over 64 rounds.</li>



<li><strong>Mixing and transforming</strong>&nbsp;: Bitwise operations, modular addition, and bit shifts mix data.</li>
</ol>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading">Examples of devices</h2>



<figure class="wp-block-table"><table class="has-fixed-layout"><thead><tr><th>Device</th><th>Hash Rate</th></tr></thead><tbody><tr><td>Bitmain Antminer S21 Pro</td><td>Up to 234 Th/s&nbsp;<a href="https://ibmm.ru/news/kriptoindustriya/algoritm-heshirovania-SHA256/" target="_blank" rel="noreferrer noopener"><sup>1</sup></a></td></tr><tr><td>Antminer T9</td><td>11.5 Th/s&nbsp;<a href="https://ibmm.ru/katalog/bitmain/T9-11_5Th/" target="_blank" rel="noreferrer noopener"><sup>4</sup></a></td></tr><tr><td>Cheetah Miner F1</td><td>About 24 Th/s&nbsp;<a href="https://pushminer.ru/produkciya/oborudovanie-dla-mainiga/asic-miners/cheetah-f1-bu" target="_blank" rel="noreferrer noopener"><sup>6</sup></a></td></tr></tbody></table></figure>



<p class="has-text-align-center has-small-font-size">These devices are optimized for maximum performance with minimal power consumption.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>To estimate the achievable performance, superconducting circuits are considered, which are currently the fastest quantum technologies and have good scaling prospects. At the maximum operating speed of elements and certain assumptions about the error rate and the complexity of the problem,&nbsp;<a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin">the effective hash rate of a quantum computer</a>&nbsp;is 13.8 GH/s, which requires the use of 4.4 million physical qubits. This is thousands of times slower than modern ASIC devices, which achieve a speed of 14 TH/s. The reason lies in the low operating speed of quantum elements and the delays associated with the creation of fault-tolerant T-elements. It is expected that quantum technologies will develop rapidly in the future, and a “quantum version of Moore’s Law” will occur, which will affect the clock rate, element accuracy and the number of qubits. This will allow us to estimate the power of quantum computers in the future.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>A quantum version of Moore’s Law</strong>&nbsp;&nbsp;is a hypothetical concept that suggests that quantum computers will experience similar increases in performance and power as classical computers do, as shown by Moore’s Law. Moore’s Law states that the number of transistors on a chip doubles every 24 months, leading to&nbsp;<a href="https://polynonce.ru/important-steps-in-the-cryptocurrency-industry-towards-quantum-electronics-in-the-era-of-moores-law/"><em>increased computing power</em>&nbsp;</a>and decreased cost. In the context of quantum computing, this increase could manifest itself in increases in the number of qubits (quantum bits), processing speed, or other parameters&nbsp;<a href="https://hub.forklog.com/kk-vs-blokchejn-chast-ii-kvantovye-ataki-na-bitkoin-i-sposoby-zashhity-ot-nih/" target="_blank" rel="noreferrer noopener"><sup>2&nbsp;</sup></a><a href="https://polynonce.ru/%D0%BA%D0%B2%D0%B0%D0%BD%D1%82%D0%BE%D0%B2%D1%8B%D0%B5-%D0%B0%D1%82%D0%B0%D0%BA%D0%B8-%D0%BD%D0%B0-%D0%B1%D0%B8%D1%82%D0%BA%D0%BE%D0%B8%D0%BD/" target="_blank" rel="noreferrer noopener"><sup>4</sup></a>&nbsp;.</p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-27-1024x761.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5211"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>It will obviously take time for quantum computers to outperform classical machines at the mining task. Even when they do, no single quantum computer will have overwhelming power. However, even a small advantage in power over other miners could make certain types of attacks profitable, such as those on mining pools that use smart contracts. For example, under certain optimistic assumptions, a group of 20 quantum machines working in parallel could have 0.1% of the total hashing power. This is enough to attack mining pools and reduce their profits by 10% with minimal bribery costs.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center">Attacks on signatures</h2>



<p>Bitcoin uses the Elliptic Curve Digital Signature Algorithm (ECDSA), based on the secp256k1 curve, to create signatures. The security of this system relies on the difficulty of the elliptic curve discrete logarithm problem&nbsp;<a href="https://cryptodeeptech.ru/discrete-logarithm/">(ECDLP)</a>&nbsp;. Although this problem is classically considered hard, Peter Shor proposed&nbsp;<em><a href="https://polynonce.ru/what-is-elliptic-curve-cryptography-ecc/">an efficient quantum algorithm to solve it</a></em>&nbsp;.&nbsp;</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-28-1024x506.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5212"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>This means that a sufficiently powerful universal quantum computer could efficiently&nbsp;<a href="https://cryptodeeptech.ru/discrete-logarithm/">compute the private key</a>&nbsp;associated with the public key, making this scheme completely insecure.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-29.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5213"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>The implications for Bitcoin are:</strong></p>



<ol class="wp-block-list">
<li><strong>(Address Reuse)</strong>&nbsp;&nbsp;In order to spend Bitcoin from an address, the public key associated with that address must be revealed. Once the public key is revealed in the presence of a quantum computer, the address is no longer secure and should therefore never be reused. While it is a best practice in Bitcoin to always use new addresses, in practice this is not always the case. Any address that contains Bitcoin and for which the public key has been revealed is completely insecure.</li>



<li><strong>(Processed transactions)</strong>&nbsp;&nbsp;If a transaction is made from an address that has not spent anything before, and that transaction is placed on the blockchain with a few blocks following it, then that transaction is reasonably secure against quantum attacks. The private key can be derived from the published public key, but since the address has already been spent, this must be combined with bypassing the network hashing to perform a double-spend attack. As we saw in Section III A, even with a quantum computer, a double-spend attack is unlikely if there are many blocks following the transaction.</li>



<li><strong>(Raw Transactions)</strong>&nbsp;&nbsp;After a transaction has been broadcast to the network, but before it is placed on the blockchain, it is at risk of a quantum attack. If the secret key can be derived from the broadcast public key before the transaction is placed on the blockchain, an attacker can use that secret key to broadcast a new transaction from the same address to their own address. If the attacker then ensures that this new transaction is placed on the blockchain first, they can effectively steal all the bitcoins behind the original address. We consider point (3) to be the most serious attack. To determine the severity of this attack, it is important to accurately estimate how long it would take a quantum computer to calculate ECDLP, and whether it can be done in a time close to the block interval.</li>
</ol>



<p>We consider the attack described in point 3 (attack on raw transactions) to be the most dangerous. To assess its severity, it is important to understand how long it would take a quantum computer to&nbsp;<a href="https://cryptodeeptech.ru/discrete-logarithm"><em>solve the Elliptic Curve Discrete Logarithm Problem</em>&nbsp;(ECDLP)</a>&nbsp;and whether it is possible to do so in a time comparable to the block generation interval in the blockchain. For an n-bit prime field, according to recent research, a quantum computer can solve the ECDLP using 9n + 2&nbsp;<em>log2(n) + 10 logical qubits and (448</em>&nbsp;log2(n) + 4090)*n^3 Toffoli gates. Bitcoin uses 256-bit signatures (n = 256), so the number of Toffoli gates is 1.28 * 10^11, which can be slightly parallelized to a depth of 1.16 * 10^11. Each Toffoli gate can be implemented using a small circuit of T-gates operating on 7 qubits in parallel (including 4 auxiliary qubits). By analyzing this, one can estimate the resources required for a quantum attack on digital signatures. As in the case of block mining, most of the time is spent on distilling the “magic states” for the logical T-gates. The time to solve ECDLP on a quantum processor is τ = 1.28 * 10^11 * cτ(pg)/s, where cτ depends only on the error rate of the gates (pg) and s is the clock frequency. The number of physical qubits required is nQ = 2334 * cnQ(pg), where the first factor is the number of logical qubits including 4 auxiliary logical qubits, and cnQ is the space cost factor.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter size-full"><a href="https://cryptodeeptech.ru/discrete-logarithm/"><img decoding="async" width="834" height="401" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-1(1).png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3238" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-1.png 834w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-1-300x144.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-1-768x369.png 768w" sizes="(max-width: 834px) 100vw, 834px"></a></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-3.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5149"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Figure&nbsp;<em>3</em>&nbsp;shows the performance of a quantum computer for attacks on digital signatures. Using a surface code with a physical gate error rate of pg = 5 * 10^-4, the overhead factors are cτ = 291.7 and cnQ = 735.3. In this case, at a clock rate of 66.6 MHz, the problem will take 6.49 days to solve, using 1.7 * 10^6 physical qubits. If the clock rate is increased to 10 GHz and the error rate is reduced to 10^-5, the signature can be cracked in 30 minutes, using 485550 qubits. The latter scenario makes an attack on raw transactions (point 3) quite possible and seriously threatens the security of the current Bitcoin system. Figure 4 presents an estimate of the time required for a quantum computer to crack the signature scheme as a function of time, based on a certain model.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>The biggest threat to Bitcoin from quantum computers is the possibility of unconfirmed transactions being stolen.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter size-full"><a href="https://cryptodeeptech.ru/vector76-attack/"><img loading="lazy" decoding="async" width="832" height="444" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-2.png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3239" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-2.png 832w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-2-300x160.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-2-768x410.png 768w" sizes="auto, (max-width: 832px) 100vw, 832px"></a></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>A quantum computer can crack a transaction signature while it is waiting to be written to the blockchain and redirect the money to the attacker’s wallet. Currently, this would require a lot of time and resources, but technological advances could make such an attack possible. To assess the danger, you need to understand&nbsp;<a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin">how quickly a quantum computer can crack these signatures</a>&nbsp;. It all depends on the computer’s power and error rate. If a sufficiently powerful and accurate quantum computer were created, it would take only half an hour to crack a signature, making the Bitcoin system very vulnerable.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-4.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5150"><figcaption class="wp-element-caption">FIGURE 4. This graph shows two estimates of the time (in seconds) it would take a quantum computer to crack the signature scheme (red curves) plotted against the next 25 years. We give more and less optimistic estimates (red striped lines). The models are described in detail in Appendix C. According to this estimate, the signature scheme could be cracked in less than 10 minutes (600 seconds, black dotted line) as early as 2027.</figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center">Future improvements to quantum attacks</h2>



<p>Attacks on the Bitcoin protocol using known quantum algorithms and error correction schemes. While some estimates of the speed and scaling of quantum computing may seem optimistic, it is important to remember that there are several ways to improve the performance of quantum computers in solving the problems mentioned. First, the error-correcting code considered here is a surface code, which requires significant classical computational overhead for state distillation, error syndrome extraction, and correction. Other codes that provide transverse Clifford and non-Clifford gates can eliminate the need for slow state distillation. In fact, the slowdown due to classical processing for syndrome extraction and correction can be completely eliminated using a dimension-free protocol such as [PSBT10], which in a recent analysis shows error thresholds [CJS16] to be only about 5 times worse than the high-dimensional surface code. This can potentially significantly improve the overall error-correction performance.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Second, reducing the number of logic gates in quantum circuits is possible as more efficient advanced quantum computing techniques are developed. For example, using a specific large-scale problem (including oracle implementations) that was analyzed in a previous paper&nbsp;<code>[SVM+17]</code>, a direct comparison of specific gate counts obtained with the Quipper software package between an old&nbsp;<code>[HHL09]</code>and new&nbsp;<code>[CKS15]</code>quantum linear system solving algorithm was achieved, showing an improvement of several orders of magnitude.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-31-1024x578.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5217"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Given that Shor’s and Grover’s quantum algorithms have been well studied and carefully optimized, one should not expect such a significant improvement, but some improvement is probably possible. Third, different quantum algorithms can provide relative speedups. A recent paper by Kaliski&nbsp;<code>[Kal17]</code>presents a quantum algorithm for&nbsp;<em><a href="https://cryptodeeptech.ru/discrete-logarithm/">the discrete logarithm problem:</a></em>&nbsp;find m given&nbsp;<a href="https://cryptodeeptech.ru/discrete-logarithm/">b = a^m</a>&nbsp;, where b is a known target value and a is a known base, using queries to a so-called “magic box” routine that computes the most significant bit of m. By repeating the queries, using carefully chosen powers of the target value, one can compute all the bits of m and solve the problem. Since different bits are solved one by one, the problem can be distributed among several quantum processors. Each processor requires a number of logical qubits comparable to solving the entire problem, but the overall time will be reduced due to parallelism. In addition, the overhead of quantum error correction is likely to be reduced since the phases in the quantum Fourier transform of part of the circuit do not have to be as precise as in Shor’s original algorithm.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-30-1024x612.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5216"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>While quantum attacks on Bitcoin seem complicated, don’t get too comfortable. There are ways to make quantum computers faster and more efficient at solving these problems.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<ul class="wp-block-list">
<li><strong>Improved error correction:</strong>&nbsp;&nbsp;Instead of using complex error correction codes, simpler and faster methods can be used that do not require continuous measurements.</li>



<li><strong>Optimizing algorithms:</strong>&nbsp;&nbsp;New quantum computing algorithms are being developed that reduce the number of operations needed to crack a signature. It’s like finding a shorter path to the goal.</li>



<li><strong>Parallelization:</strong>&nbsp;&nbsp;The hacking task can be divided into parts and distributed among several quantum computers to speed up the process.</li>
</ul>



<p>So, even if a quantum attack on Bitcoin now requires huge resources, as technology develops, this threat will become more and more real.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center">COUNTERMEASURES: Alternative proofs-of-work</h2>



<p>A quantum computer can use Grover’s search to perform Bitcoin’s proof-of-work using quadratically fewer hashes than classically required. In this section, we explore alternative proofs-of-work that may offer a smaller quantum advantage. The main properties we want from proof-of-work are:</p>



<ol class="wp-block-list">
<li><strong>(Difficulty)</strong>&nbsp;&nbsp;The difficulty of the task can be adjusted according to the computing power available on the network.</li>



<li><strong>(Asymmetry)</strong>&nbsp;&nbsp;It is much easier to verify that a proof-of-work has completed successfully than to perform a proof-of-work.</li>



<li><strong>(No quantum advantage)</strong>&nbsp;&nbsp;Proof-of-work cannot be performed significantly faster on a quantum computer than on a classical computer.</li>
</ol>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-34.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5220"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Python script:&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/QuantumInspiredPoW.py" target="_blank" rel="noreferrer noopener">QuantumInspiredPoW.py</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-a6943f49ad156aae464fc8259396a45d" style="color:#4092c2"><code><strong>import hashlib
import random

def rough_hash_check(nonce, prefix_zeros):
    """
    Simulates checking a hash for compliance with difficulty (number of zeros at the beginning).
    """
    data = str(nonce).encode('utf-8')
    hash_value = hashlib.sha256(data).hexdigest()
    return hash_value.startswith('0' * prefix_zeros)

def grover_proof_of_work(difficulty):  # difficulty - number of zeros at the start of the hash
    """
    Pseudocode demonstrating an attempt to apply Grover's search idea 
    (quantum acceleration of search) to find a nonce that meets 
    Proof-of-Work requirements. In practice, this will not provide significant 
    acceleration on a classical computer.
    """
    N = 2**32  # Example: nonce search space (simplified)
    
    iterations = int(N**0.5)  # Square root of N - estimate of Grover's iterations

    for _ in range(iterations):
        random_nonce = random.randint(0, N - 1) # Random choice of nonce
        if rough_hash_check(random_nonce, difficulty):
            print(f"Found nonce: {random_nonce}")
            return random_nonce
    return None  # Did not find a suitable nonce

# Example usage (with very low difficulty to find something)
difficulty = 2
nonce = grover_proof_of_work(difficulty)

if nonce:
    print(f"Nonce satisfying difficulty {difficulty}: {nonce}")
else:
    print("Failed to find a nonce within the specified number of iterations.")

</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<ol class="wp-block-list">
<li>brute force hash check&nbsp;<code>(nonce, prefix_zeros)</code>: This function simulates checking whether the nonce hash matches a given difficulty (the number of leading zeros in the hash). In the real Bitcoin network, this is replaced by checking that the block header hash (including the nonce) is less than a target value.&nbsp;<a href="https://python-scripts.com/blockchain">This uses</a>&nbsp;<code>hashlib.sha256</code>&nbsp;.</li>



<li>Grover search&nbsp;<code>proof_of_work(difficulty)</code>: This is the main function that tries to find a nonce that satisfies the PoW requirements.
<ul class="wp-block-list">
<li><code>N = 2**32</code>: Represents the nonce search space. In the real Bitcoin network, the search space is much larger.</li>



<li><code>iterations = int(N**0.5)</code>: The key idea is inspired by Grover’s algorithm. Grover’s algorithm theoretically allows finding a solution in a search space of size N&nbsp;<code>O(sqrt(N))</code>operations, as opposed to O(N) for exhaustive search. We try to reflect this by performing the square root of N iterations.</li>



<li>In the loop, we randomly select a nonce and check if its hash meets the difficulty requirements.</li>
</ul>
</li>



<li>Note that this code&nbsp;&nbsp;<strong>is not a real implementation of Grover’s algorithm</strong>&nbsp;&nbsp;and will not give any speedup on a classical computer. It simply demonstrates the concept of using&nbsp;<code>sqrt(N)</code>iterations.</li>
</ol>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-35-1024x669.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5222"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Bitcoin’s proof-of-work satisfies (1) and (2), but we would like to find an alternative proof-of-work that does (3) better. Similar considerations have been explored by authors trying to find proofs-of-work that, instead of (3), look for proofs-of-work that cannot be accelerated by ASICs. An approach to this is to consider memory-intensive proofs-of-work. Several interesting candidates have been proposed, such as&nbsp;<a href="https://keyhunters.ru/quantum-resistance-and-momentum-algorithm/">Momentum</a>&nbsp;[Lar14], which is based on finding collisions in a hash function, Cuckoo Cycle [Tro15], which is based on finding constant-size subgraphs in a random graph, and Equihash [BK17], which is based on the generalized birthday problem. These are also good candidates for a more quantum-resistant proof-of-work. All of these schemes are based on hashcash-style proof-of-work and use the following template. Let be&nbsp;<code>h1 : {0, 1} ∗ → {0, 1} n</code>a cryptographically secure hash function and H = h1(header) be the hash of the block header. The goal is to find a nonce x such that&nbsp;<code>h1(H k x) ≤ t и P(H, x)</code>for some predicate P.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-36-1024x595.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5226"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>The fact that the header and nonce must satisfy the predicate P means that the best algorithm will no longer simply iterate over nonce x. Having proof-of-work in this form also ensures that the parameter t can still be chosen to vary the difficulty. We next analyze this pattern for proof-of-work Momentum, as this can be related to known quantum lower bounds. For proof-of-work Momentum, let h2 : {0, 1} ∗ → {0, 1} be another hash function with n ≤ . In the original Momentum proposal, h1 could be taken to be SHA-256 and h2 to be a memory-intensive hash function, but this is less important for our discussion. The proof-of-work is to find H, a, b such that h1(H kakb) ≤ t and h2(H ka) = h2(H kb) and a, b ≤ 2 `. (1)Let us first examine the running time for solving this proof-of-work, assuming that the hash functions h1, h2 can be evaluated in unit time. Taking a subset S ⊂ {0, 1} and evaluating h2(H ka) for all a ∈ S, we expect to find about |S| 2/2 many collisions. Note that, using an appropriate data structure, these collisions can be found in about |S| time. One algorithm then is as follows. For each H, we evaluate h2 on the subset S and find about |S| 2/2 many pairs a, b such that h2(H ka) = h2(H kb).</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter size-full"><a href="https://cryptodeeptech.ru/rowhammer-attack/"><img loading="lazy" decoding="async" width="833" height="409" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-3(1).png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3240" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-3.png 833w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-3-300x147.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-3-768x377.png 768w" sizes="auto, (max-width: 833px) 100vw, 833px"></a></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>For each collision, we then test h1(H kakb) ≤ t. In anticipation, we will have to perform this second test 2n/t many times. So the number of H’s we will have to try is about m = max{1, 2 n+ t|S| 2 }, since we must try at least one H. Since we spend |S| time for each H, the total running time is m|S|. We see that it is smallest when |S| = q 2 n+ t , that is, when m = 1 and we just try one H. This optimal running time is then T = q 2 n+ t , and to achieve it we must use memory equal to the running time, which can be prohibitively expensive. For some smaller memory |S| &lt; q 2 n+ t the running time will be 2 n++1 t|S| . Now let’s look at the running time on a quantum computer. On a quantum computer, we can do the following. We call H good if there exist a, b ∈ S such that h1(H kakb) ≤ t and h2(H ka) = h2(H kb). Checking whether H is good requires finding a collision and hence requires at least |S| 2/3 time according to the quantum lower bound of queries of Aaronson and Shi [AS04].</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-37-1024x583.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5227"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><em>Note</em>&nbsp;that this lower bound is tight, since finding such a collision can also be done in about |S| 2/3 time using the Ambainis Element Dissimilarity Algorithm [Amb07]. We argued above that finding at least one good H requires a set of size m = max{1, 2 n+ t|S| }. From Grover’s search optimality [BBBV97], we know that we must perform at least √ m many tests to find a good H. Since checking whether H is good takes |S| 2/3 time, the total running time is at least √ m|S| 2/3 . Since the classical running time is m|S|, we see that, unlike the current proof-of-work in Bitcoin, with this proposal a quantum computer will not be able to achieve a quadratic advantage once S becomes larger than a constant size. In particular, since √ m|S| 2/3 is also minimized when S = q 2 n+ t , the execution time of even the fastest quantum algorithm is at least T 2/3 , which is significantly larger than T 1/2 .</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em><a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin">Quantum computers</a>&nbsp;can solve Bitcoin’s current proof-of-work problem faster. Therefore, alternative ways of securing the blockchain that will be more resistant to quantum attacks are being sought. One approach is to use proof-of-work, which requires large amounts of memory.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Examples:&nbsp;<a href="https://cryptodeeptech.ru/publication">Momentum, Cuckoo Cycle, Equihash</a>&nbsp;. These methods make the task more difficult for quantum computers. The basic idea is to find a number (nonce) that satisfies certain conditions. These conditions are related to finding collisions in hash functions. The&nbsp;<a href="https://keyhunters.ru/quantum-resistance-and-momentum-algorithm">Momentum</a>&nbsp;algorithm , for example, requires finding two different values ​​that give the same result when hashed. Unlike the current proof-of-work in Bitcoin, with such alternative approaches, a quantum computer does not gain a big advantage. The time required to solve the problem increases, making the attack less profitable.</p>



<p>Finding collisions in hash functions, especially in the context of the Momentum algorithm (as described in theoretical papers on quantum stability of PoW), usually comes down to the following:</p>



<ol class="wp-block-list">
<li><strong>Defining hash functions:</strong>&nbsp;&nbsp;It is necessary to define the hash functions in which collisions are to be found (h1 and h2 in the context of Momentum PoW). In real systems, this could be SHA256 or other cryptographic hash functions.</li>



<li><strong>Implementation of collision detection:</strong>&nbsp;&nbsp;Various methods can be used to detect collisions, from simple (brute-force) to more complex (e.g.&nbsp;<a href="https://keyhunters.ru/steps-in-a-birthday-attack-on-bitcoin">birthday attack</a>&nbsp;).</li>
</ol>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-38.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5228"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p class="has-medium-font-size">Here is an example Python script demonstrating brute-force collision detection for a simplified hash function (&nbsp;&nbsp;<strong>insecure</strong>&nbsp;for demonstration purposes ):</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Python script:&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/CollisionHunter.py" target="_blank" rel="noreferrer noopener">CollisionHunter.py</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-460cf49ce80c6a22dd14e4c8aa89db70" style="color:#4092c2"><code><strong>import hashlib
import random

def simple_hash(data, modulus):
    """
    Simplified hash function for demonstration.
    DO NOT USE IN PRODUCTION.
    """
    data_bytes = str(data).encode('utf-8')  # Convert to bytes
    hash_value = int(hashlib.sha256(data_bytes).hexdigest(), 16) % modulus
    return hash_value

def find_collision(hash_function, modulus, max_attempts=100000):
    """
    Finds a collision for a given hash function and modulus.
    """
    seen_hashes = {}
    for i in range(max_attempts):
        data = random.randint(0, modulus * 10)  # Generate random data
        hash_value = hash_function(data, modulus)

        if hash_value in seen_hashes:
            data1 = seen_hashes[hash_value]
            data2 = data
            print(f"Collision found: data1={data1}, data2={data2}, hash={hash_value}")
            return data1, data2, hash_value
        else:
            seen_hashes[hash_value] = data

    print("No collision found within the specified number of attempts.")
    return None

# Example usage
modulus = 256  # Size of the hash table (for example)
collision = find_collision(simple_hash, modulus)

if collision:
    data1, data2, hash_value = collision
    print(f"Data 1: {data1}, Data 2: {data2}, Hash: {hash_value}")
</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>What this script does:</strong></p>



<ol class="wp-block-list">
<li><code>simple_hash(data, modulus)</code>: A simplified hash function. It takes the SHA256 of the data, converts the hash to an integer, and takes the remainder when divided by&nbsp;&nbsp;<code>modulus</code>.&nbsp;&nbsp;<strong>Important:</strong>&nbsp;&nbsp;This hash function is for demonstration purposes only. It is not cryptographically secure. Do not use it in real applications.</li>



<li><code>find_collision(hash_function, modulus, max_attempts=100000)</code>: This function tries to find a collision for a given hash function. It generates random data, calculates its hash and stores it in a dictionary&nbsp;&nbsp;<code>seen_hashes</code>. If the generated hash is already in the dictionary, then we have found a collision.</li>



<li>In the usage example, we set the hash table size (&nbsp;<code>modulus</code>) to 256 and run a collision search.</li>



<li>This code looks for collisions “head-on”, that is, it simply iterates through random values ​​and checks whether such a hash has already existed. This method only works for very simple hash functions with a small output range.</li>
</ol>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Key points and warnings:</strong></p>



<ul class="wp-block-list">
<li><strong>Insecurity&nbsp;&nbsp;<code>simple_hash</code>:</strong>&nbsp;&nbsp;The hash function&nbsp;&nbsp;<code>simple_hash</code>&nbsp;is extremely vulnerable to attacks and is not suitable for real cryptographic tasks. It is used only to demonstrate the principle of finding collisions.</li>



<li><strong>Collision Finding Difficulty:</strong>&nbsp;&nbsp;Finding collisions for cryptographically strong hash functions such as SHA256 is an extremely difficult task. A brute-force search is impossible due to the huge size of the hash function output space.</li>



<li><strong><a href="https://keyhunters.ru/steps-in-a-birthday-attack-on-bitcoin">Birthday attack:</a></strong>&nbsp;&nbsp;A more efficient method for finding collisions (compared to a complete search) is the birthday attack. This method is based on the birthday paradox and allows finding a collision in approximately&nbsp;<code>sqrt(N)</code>&nbsp;operations, where&nbsp;<code>N</code>&nbsp;is the size of the output space of the hash function. However, even for the birthday attack, huge computing resources are required for SHA256.</li>



<li><strong><a href="https://keyhunters.ru/quantum-resistance-and-momentum-algorithm">Momentum Algorithm</a>&nbsp;:</strong>&nbsp;&nbsp;Implementing the Momentum algorithm would require also implementing h2 and the validation logic&nbsp;<code>h1(H k a k b) ≤ t</code>.</li>



<li><strong>Resources to learn:</strong>&nbsp;&nbsp;Check out ”&nbsp;<a href="https://javarush.com/quests/lectures/ru.javarush.python.core.lecture.level16.lecture06">Collision Problems and Solutions</a>&nbsp;“, ” Hash Tables in Python: How They Work and Why You Need Them “, ”&nbsp;<a href="https://keyhunters.ru/list-with-hash-collisions/">List with Hash Collisions</a>&nbsp;“, and more to gain a deeper understanding of the problem.</li>
</ul>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p class="has-medium-font-size">This example serves as a starting point. For more complex scenarios (e.g. birthday attack or integration with Momentum)&nbsp;</p>


<div class="wp-block-image">
<figure class="aligncenter size-full"><a href="https://cryptodeeptech.ru/signature-malleability/"><img loading="lazy" decoding="async" width="832" height="416" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-4(1).png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3241" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-4.png 832w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-4-300x150.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-4-768x384.png 768w" sizes="auto, (max-width: 832px) 100vw, 832px"></a></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin">Post-quantum signature schemes</a></h2>



<p>Numerous public-key digital signature schemes have been proposed in the literature that are supposedly resistant to quantum computers. Examples include hashing-based schemes (LMS, XMSS, SPHINCS, NSW), code-based schemes (CFS, QUARTZ), multivariate polynomial-based schemes (RAINBOW), and lattice-based schemes (GPV, LYU, BLISS, DILITHIUM, NTRU). Each of these cryptosystems has varying degrees of efficiency. A comparison of signature and key sizes is presented in Table II (in the original text). In the context of blockchain, the most important parameters of a signature scheme are the length of the signature and the public key, since they must be stored somewhere to fully verify transactions, and the signature verification time.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-5-1024x410.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5153"><figcaption class="wp-element-caption">According to Table II, in terms of the sum of the signature and public key lengths, the only reasonable options are hashing and lattice-based schemes.</figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Hash-based schemes like XMSS have the advantage of being provably secure, at least if the chosen hash function behaves like a random oracle. A common quantum attack on these schemes is to use Grover’s algorithm, which means their quantum security is half their classical security.</p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-15-1024x588.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5194"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>In contrast, the best known quantum attack on DILITHIUM at 138-bit classical security level requires 2^125 time. Thus, for the same quantum security level, lattice-based schemes have some advantage in signature length plus public key.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-16-1024x335.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5196"></figure></div>


<p>Although the lattice-based BLISS scheme has the smallest sum of signature and public key lengths of all the schemes in Table II, there are several reasons not to choose BLISS in practice. The security of BLISS is based on the difficulty of the NTRU problem and the assumption that solving this problem is equivalent to finding a short vector in the so-called NTRU lattice. It has recently been shown that this assumption may be too optimistic, at least for large parameters. Moreover, there is a history of attacks on previous NTRU-based signature schemes. Perhaps most importantly, BLISS is difficult to implement securely because it is highly susceptible to side-channel attacks. The production BLISS implementation strongSwan was attacked in this way by Pessl et al., who showed that the signature key can be recovered after observing approximately 6000 signature generations.</p>


<div class="wp-block-image">
<figure class="aligncenter size-full"><a href="https://cryptodeeptech.ru/lattice-attack-249bits/"><img loading="lazy" decoding="async" width="837" height="407" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-5.png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3242" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-5.png 837w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-5-300x146.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-5-768x373.png 768w" sizes="auto, (max-width: 837px) 100vw, 837px"></a></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>When it comes to protecting against quantum computers, there are many different ways to encrypt data. The most popular methods include using hash functions and mathematical lattices.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<ul class="wp-block-list">
<li><strong>Hash functions:</strong>&nbsp;&nbsp;This method is good because it can be proven secure, but quantum computers can speed up the cracking of this cipher a little.</li>



<li><strong>Lattice:</strong>&nbsp;&nbsp;This method looks more promising in terms of protection against quantum computers, but it has its drawbacks. For example, the lattice-based BLISS algorithm is very vulnerable to attacks that use information about the computer’s operation (such as power consumption) to steal the key.</li>
</ul>



<hr class="wp-block-separator has-alpha-channel-opacity">



<figure class="wp-block-image"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-6-1024x595.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5154"><figcaption class="wp-element-caption">TABLE III. Algorithms for computing space and time resources for quantum attacks. Input<br>pg, the error rate of the physical gate; nC, the total number of Clifford gates in the logic circuit; nT, the total number of T gates in the logic circuit; and nL, the number of logical qubits. Output<br>τ, the time cost in cycles; and nQ = Qcircuit + Qfactory, the number of<br>physical qubits used for the computation, including state distillation.</figcaption></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center">Estimating the Error Correction Overhead in a Quantum Attack</h2>



<p>How are quantum error correction overhead factors calculated to obtain resource cost estimates for&nbsp;<a href="https://cryptodeeptech.ru/publication">quantum attacks</a>&nbsp;on blockchains and digital signatures? The method is based on the analysis in [FMMC12, MDMG+16]. First, nT and nC are determined, which are the numbers of T-gates and Clifford gates required in the algorithm. The pseudocode for calculating the overhead is presented in Table III (in the original text).</p>



<ul class="wp-block-list">
<li>For an attack on a blockchain with nL = 2402 qubits, these values ​​are nT = 297784 × π^2 / (14√(10) · D), nC = 29.4 × nT.</li>



<li>For a digital signature attack with nL = 2334 qubits, the values ​​are nT = 1.28 × 10^11, nC = 20 × nT.</li>
</ul>



<p>Looking ahead a few years, we can assume plausible improvements in quantum computer technology. Assuming a quantum error correction code that supports Clifford and non-Clifford transversal gates, so there is no distillation slowdown, and that this is done without measurement, so no classical error syndrome handling is required, then the number of cycles required for one oracle call is determined solely by the circuit depth, which is 2142094. This is based on the total circuit depth, calculated as follows. The oracle makes two calls to the SHA256 hash function, and it does this twice: once to compute it and once to undo it. Each hash has a reversible circuit depth of 528768. Similarly, two multi-gate phase gates are used, one for mean inversion and one for function call, each of which has a circuit depth of 13511, for a total depth of 4 × 528768 + 2 × 13511 = 2142094 (these numbers are taken from [SFL+13] but can be further optimized). Then, accepting the potential overhead in space and number of physical qubits, but assuming no time overhead for error correction or distillation of non-Clifford gates, this implies an improved effective hash rate of hQC = 0.04 × s / √D, which is substantially faster. For superconducting circuits, ultrafast geometric phase gates are possible at ∼50 GHz, which is mainly limited by the microwave cavity frequency [RBW+12]. Using the above very optimistic assumptions, at difficulty D = 10^12 the effective hash rate is hQC = 2.0 × 10^3 TH/s.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-21-1024x473.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5204"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>To estimate how much resources are needed for a quantum attack on a blockchain or digital signatures, many factors need to be taken into account, including the number of certain quantum operations (T-gates and Clifford gates) and the error correction methods in a quantum computer. Assuming that quantum computers become better in the future and can quickly and efficiently correct errors, the speed of hacking (hash rate) could increase significantly.</em></p>



<p>It is important to understand that these scripts are intended to&nbsp;&nbsp;<strong>simulate</strong>&nbsp;&nbsp;quantum computing on a classical computer, since running on a real quantum computer requires specialized hardware and access to it.</p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-19-1024x347.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5201"></figure></div>


<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><strong>Example 1: Qiskit (IBM)</strong>&nbsp;Qiskit is one of the most popular libraries for quantum programming in Python<sup>&nbsp;<a href="https://habr.com/ru/companies/yandex/articles/510054/" target="_blank" rel="noreferrer noopener">2&nbsp;</a><a href="https://vc.ru/dev/88875-ispolzovanie-kvantovyh-ventilei-v-biblioteke-qiskit-na-python-chast-pervaya" target="_blank" rel="noreferrer noopener">3&nbsp;</a><a href="https://sky.pro/media/kak-ispolzovat-python-dlya-raboty-s-kvantovymi-kompyuterami/" target="_blank" rel="noreferrer noopener">7</a></sup>&nbsp;. It provides tools for creating, simulating, and executing quantum circuits.</p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Python script:&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/QuBitWizard.py" target="_blank" rel="noreferrer noopener">QuBitWizard.py</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-f7f7757716b43f96a1bee4329b016d7d" style="color:#4092c2"><code><strong>from qiskit import QuantumCircuit, transpile
from qiskit.quantum_info import Statevector
from qiskit.visualization import plot_histogram

# Create a quantum circuit with 2 qubits and 2 classical bits
circuit = QuantumCircuit(2, 2)

# Apply the Hadamard gate (H, Clifford) to the first qubit
circuit.h(0)

# Apply the CNOT gate (Clifford) with control qubit 0 and target qubit 1
circuit.cx(0, 1)

# Add a T-gate (non-Clifford) to qubit 0
circuit.t(0)

# Measure the qubits and store results in classical bits
circuit.measure([0, 1], [0, 1])

# Simulate the circuit
simulator = Aer.get_backend('qasm_simulator') # Use Aer for simulation
compiled_circuit = transpile(circuit, simulator) # Transpile the circuit 
job = simulator.run(compiled_circuit, shots=1000) # Run simulation for 1000 times 
result = job.result() # Get results 
counts = result.get_counts(circuit) # Get measurement statistics

print(counts) # Print results 
plot_histogram(counts) # Display histogram of results (requires matplotlib)
<code>
</code></strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>In this example:</strong></p>



<ul class="wp-block-list">
<li><code>QuantumCircuit(2, 2)</code>: Creates a quantum circuit with 2 qubits and 2 classical bits to store measurement results.</li>



<li><code>circuit.h(0)</code>: Applies the Hadamard gate (H) to qubit 0. The Hadamard gate creates a superposition, putting the qubit in the state (|0⟩ + |1⟩)/√2&nbsp;<a href="https://tproger.ru/articles/kvantovye-yazyki-programmirovaniya" target="_blank" rel="noreferrer noopener"><sup>1</sup></a>&nbsp;. H is a Clifford gate.</li>



<li><code>circuit.cx(0, 1)</code>: Uses a CNOT (Controlled-NOT) gate with control qubit 0 and target qubit 1. CNOT is a Clifford gate.</li>



<li><code>circuit.t(0)</code>: Applies the T-gate to qubit 0. The T-gate is a non-Clifford gate and plays an important role in universal quantum computation.</li>



<li><code>circuit.measure([0, 1], [0, 1])</code>: Measures the state of qubits 0 and 1 and stores the results in classical bits 0 and 1 respectively.</li>



<li><code>Aer.get_backend('qasm_simulator')</code>: Gets the QASM (Quantum Assembly Language) simulator from Aer (Quantum’s framework for simulating quantum computing).</li>



<li><code>transpile(circuit, simulator)</code>: Optimizes a quantum circuit for a given simulator.</li>



<li><code>simulator.run(compiled_circuit, shots=1000)</code>: Runs the simulation 1000 times (shots).</li>
</ul>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-18-1024x380.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5200"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><strong>Example 2:&nbsp;</strong><a href="https://polynonce.ru/pip-install-pyquil/"><strong>pyQuil (Rigetti)</strong>&nbsp;pyQuil</a>&nbsp;is a library from Rigetti Computing focused&nbsp;<a href="https://polynonce.ru/how-quantum-programming-languages-work/">on superconducting quantum computers.</a></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Python script:&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/WaveMaster.py" target="_blank" rel="noreferrer noopener">WaveMaster.py</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-b4604e3f1fd41580421b53a71ef27a15" style="color:#4092c2"><code><strong>from pyquil import Program
from pyquil.gates import H, CNOT, T
from pyquil.api import WavefunctionSimulator

# Create a quantum program
program = Program()

# Apply the Hadamard gate to qubit 0
program += H(0)

# Apply CNOT with control qubit 0 and target qubit 1
program += CNOT(0, 1)

# Apply the T gate to qubit 0
program += T(0)

# Create a simulator
simulator = WavefunctionSimulator()

# Simulate the program and get the wave function
wavefunction = simulator.simulate(program)

# Print the wave function
print(wavefunction)<code>
</code></strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>In this example:</strong></p>



<ul class="wp-block-list">
<li><code>Program()</code>: Creates an object representing a quantum program.</li>



<li><code>H(0)</code>,&nbsp;&nbsp;<code>CNOT(0, 1)</code>,&nbsp;&nbsp;<code>T(0)</code>: Applies Hadamard, CNOT, and T gates to the specified qubits.</li>



<li><code>WavefunctionSimulator()</code>: Creates a quantum computing simulator.</li>



<li><code>simulator.simulate(program)</code>: Simulates the execution of a program and returns a wave function describing the state of the qubits after the program has executed.</li>
</ul>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<figure class="wp-block-image"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-17-1024x618.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5199"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">
</blockquote>



<p><strong>Python script:&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/CirqQuantumCircuit.py" target="_blank" rel="noreferrer noopener">CirqQuantumCircuit.py</a></strong></p>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Example 3: Cirq (Google)</strong></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-00d82d61f50918158f2f96a4a33cb9a4" style="color:#4092c2"><code><strong>import cirq

# Create qubits
qubit1 = cirq.GridQubit(0, 0)
qubit2 = cirq.GridQubit(0, 1)

# Create circuit
circuit = cirq.Circuit()

# Add operations
circuit.append(cirq.H(qubit1))
circuit.append(cirq.CNOT(qubit1, qubit2))
circuit.append(cirq.T(qubit1))

# Simulate circuit
simulator = cirq.Simulator()
result = simulator.simulate(circuit)

print(circuit)
print(result)</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>In this example, Cirq is used for the same operations as in the previous examples, but using Cirq syntax.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>Important notes:</strong></p>



<ul class="wp-block-list">
<li><strong>Installing libraries:</strong>&nbsp;&nbsp;Before running these scripts, you need to install the corresponding libraries. For example, for Qiskit:&nbsp;&nbsp;<code>pip install qiskit qiskit-aer qiskit-visualization</code>. For&nbsp;<a href="https://polynonce.ru/pip-install-pyquil/">pyQuil</a>&nbsp;:&nbsp;&nbsp;<code>pip install pyquil</code>. For Cirq:&nbsp;&nbsp;<code>pip install cirq</code>.</li>



<li><strong>Quantum Simulators:</strong>&nbsp;&nbsp;These libraries use classical computers to simulate quantum computations. The simulation is computationally intensive and its capabilities are limited compared to real quantum computers.</li>



<li><strong>Universality:</strong>&nbsp;&nbsp;Clifford gates and T-gates (or other non-Clifford gates) constitute a universal set of gates. This means that any quantum circuit can be approximated using only these gates.</li>
</ul>



<p>These examples provide a starting point for experimenting with quantum operations (including T-gates and Clifford gates) using Python and quantum libraries.</p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>For example, if certain technologies and very optimistic forecasts are used, the hash rate can reach enormous values, which will greatly simplify quantum attacks.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter size-full"><a href="https://cryptodeeptech.ru/signature-malleability/"><img loading="lazy" decoding="async" width="827" height="401" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-6.png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3246" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-6.png 827w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-6-300x145.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-6-768x372.png 768w" sizes="auto, (max-width: 827px) 100vw, 827px"></a></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center">Modeling the evolution of hashrate and difficulty of the Bitcoin network</h2>



<p>The total number of hashes per second across the entire Bitcoin network is taken from blockchain.info. The data in Figure 5(a) are the hash rates as of January 1st (2012–2015) and January 1st and July 1st (2016–2017). The two dashed curves represent optimistic and less optimistic assumptions for the extrapolations. The optimistic extrapolation assumes that the current growth will continue exponentially for five years and then become linear as the market is saturated with fully optimized Bitcoin ASIC miners. The less optimistic assumption assumes linear growth at the current rate. By extrapolating the Bitcoin network hash rate, the difficulty can be determined as a function of time. The expected number of hashes needed to find a block in 10 minutes (600 seconds) is given by rate(t) * 600, where rate(t) is the overall hash rate shown in Figure 5(a). Thus, Bitcoin’s hashing difficulty is calculated as D(t) = rate(t) * 600 * 2^(-32) for the two scenarios described above. Figure 5(b) compares this with the values ​​from blockchain.info for January 1, 2015–2017.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>To predict how Bitcoin mining difficulty will change, they analyze how quickly the network’s computing power (hashrate) is growing. Hashrate data is taken from the blockchain.info website and graphs are built showing how the hashrate has changed in the past.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-13-1024x373.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5174"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Two predictions are made:</strong></p>



<ol class="wp-block-list">
<li><strong>Optimistic:</strong>&nbsp;&nbsp;The hashrate will continue to grow very quickly until everyone switches to the latest miners.</li>



<li><strong>Less optimistic:</strong>&nbsp;&nbsp;The hashrate will grow at the same rate as now.</li>
</ol>



<p>Using these predictions, you can calculate how&nbsp;<a href="https://bits.media/difficulty/bitcoin/">difficult it will be to mine Bitcoin in the future</a>&nbsp;. Difficulty is calculated based on how many hashes it takes to find a new block&nbsp;<a href="https://bits.media/hashrate/" target="_blank" rel="noreferrer noopener">1</a>&nbsp;.&nbsp;&nbsp;<em><a href="https://keyhunters.ru/bitcoin-hashrate-reaches-all-time-high-contrary-to-analyst-expectations/">The higher the hash rate, the higher the difficulty</a></em>&nbsp;.</p>


<div class="wp-block-image">
<figure class="aligncenter is-resized"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-14.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5178" style="width:840px;height:auto"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin">Modeling the development of quantum computers</a></h2>



<p>There are several aspects of quantum technology development that need to be taken into account in the modeling. Since only a few data points are available at this early stage of development, there is inevitably a large uncertainty in our estimates. We therefore provide two different estimates: one that is optimistic about the rate of development, and one that is significantly more pessimistic. However, these projections should be considered as very rough estimates that may require adjustment in the future. First, we need to make an assumption about the number of qubits available at any given time. Since we are focusing only on solid-state superconducting implementations, there are only a few data points available.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-9(1).png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5159"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>We assume that the number of available qubits will grow exponentially over time in the near future. An optimistic assumption is that the number will double every 10 months, while a less optimistic assumption is that the number will double every 20 months. These two extrapolations are shown in&nbsp;<em>Figure 6</em>&nbsp;(a). The data points are taken from the following table: (table not shown).</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-8.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5158"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Predicting the development of quantum computers is difficult because we have little information yet. Therefore, the authors of the article made two predictions that differ from each other:</p>



<ul class="wp-block-list">
<li><strong>Optimistic forecast:</strong>&nbsp;&nbsp;Quantum computers will develop very quickly, and the number of qubits (the basic “building blocks” of quantum computing) will double every 10 months.</li>



<li><strong>Pessimistic forecast:</strong>&nbsp;&nbsp;The development of quantum computers will proceed more slowly, and the number of qubits will double every 20 months.</li>
</ul>



<p>Both predictions are likely not very accurate, but they help us understand how quickly quantum computers can develop and when they might become a threat to existing information security systems.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>We predict that the quantum gate frequency will grow exponentially over the next few years. This assumes that classical control schemes will be fast enough to drive quantum gates at these frequencies. After a couple of years, the growth slows down significantly, as faster classical control schemes are needed to further speed up quantum gates. We limit the quantum gate frequency to 50 GHz (for the optimistic case) or 5 GHz (for the less optimistic case), respectively, mainly because we expect that classical control schemes will not be able to drive quantum gates at higher frequencies. (See, for example,&nbsp;<code>[HHOI11]</code>progress in this direction.)</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-10.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5160"><figcaption class="wp-element-caption">This is shown in Figure 6(b). The data points are taken from the following table: (table not shown).</figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>The paper also predicts how fast quantum computers will operate, that is, how often they will be able to perform basic operations (quantum gates).</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter size-full"><a href="https://cryptodeeptech.ru/twist-attack/"><img loading="lazy" decoding="async" width="833" height="475" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-7.png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3248" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-7.png 833w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-7-300x171.png 300w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-7-768x438.png 768w" sizes="auto, (max-width: 833px) 100vw, 833px"></a></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<ul class="wp-block-list">
<li><strong>Forecast:</strong>&nbsp;&nbsp;At first, the speed of quantum computers will grow very quickly, but then the growth will slow down.</li>



<li><strong>Limitation:</strong>&nbsp;&nbsp;The authors believe that there is a speed limit that will be difficult to exceed because quantum computers require very fast “regular” (classical) computers to operate. If regular computers cannot keep up, then quantum computers will not be able to operate faster.</li>
</ul>



<p>The optimistic forecast suggests that the operating speed of quantum computers will reach 50 GHz, while the pessimistic one suggests only 5 GHz.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-11.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5162"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Figure 6 shows the predicted number of qubits, the gate frequency (in gate operations per second), and the gate imprecision as a function of time. The fourth plot models the reduction in overhead due to theoretical advances. The predicted evolution of gate imprecision is shown in Figure 6(c). We assume that gate imprecision will continue to decrease exponentially, but that this evolution will stop at an imprecision of 5 × 10^-6 (optimistic case) or 5 × 10^-5 (less optimistic case). For the optimistic case, we expect gate imprecision to continue to follow DiVincenzo’s law, which predicts imprecision to decrease by a factor of 2 per year. The data are taken from the following table: (table not shown).</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-12.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5164"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>In addition to the number of qubits and how fast they operate, it is important to consider how well they work, that is, how often they make mistakes.</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>This is called&nbsp;<strong>“valve inaccuracy”</strong>&nbsp;.</p>



<ul class="wp-block-list">
<li><strong>Prediction:</strong>&nbsp;&nbsp;Quantum computers are expected to become more accurate and the number of errors will decrease.</li>



<li><strong>Limitation:</strong>&nbsp;&nbsp;But there is a limit beyond which it will be very difficult to improve accuracy. The optimistic forecast assumes that the inaccuracy will decrease to 5 per million, and the pessimistic one – to 5 per 100 thousand.</li>
</ul>



<p>The more accurately the qubits work, the less additional resources (qubits and time) are needed to correct errors.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Finally, we expect the number of qubits and time steps required by any algorithm to decrease over time for two reasons.&nbsp;<em>First</em>&nbsp;, the precision of the gates will increase over time, allowing for more efficient fault-tolerant circuits.&nbsp;<em>Second</em>&nbsp;, theoretical advances will allow the number of qubits and gates required to implement the algorithm and fault-tolerant circuits to decrease. We expect this factor to be&nbsp;<code>overhead(t) = β^(t-2017)</code>, where&nbsp;<code>β ∈ {0.75, 0.85}</code>for optimistic and less optimistic assumptions, respectively.</p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-23-1024x468.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5207"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size"><em>Over time, solving problems on quantum computers will require fewer resources (qubits and time) due to two things:</em></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<ol class="wp-block-list">
<li><strong>Improving qubit accuracy:</strong>&nbsp;&nbsp;The more accurate qubits are, the less additional effort is needed to correct errors.</li>



<li><strong>Theoretical breakthroughs:</strong>&nbsp;&nbsp;Scientists will develop new algorithms and methods that will allow the same calculations to be done using fewer qubits and operations.</li>
</ol>



<p>To estimate how much the resource requirements will be reduced, they introduce a special coefficient that depends on time and how optimistic we are about the future. This coefficient shows how many times the number of required qubits and time can be reduced.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://colab.research.google.com/drive/1jqHX5Oawy3QPh2OSYVf6AF1RGtjAb4rj?usp=sharing" target="_blank" rel="noreferrer noopener">The process of identifying a critical vulnerability in a transaction</a></h2>


<ol class="wp-block-footnotes"><li id="77e87faf-f7a7-4a3c-b1f8-1e4690c475ac"> <a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin-assessing-vulnerabilities-and-developing-defense-strategies-against-emerging-quantum-computing-threats/#77e87faf-f7a7-4a3c-b1f8-1e4690c475ac-link" aria-label="Jump to footnote reference 1">↩︎</a></li></ol>


<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-text-align-left has-medium-font-size"><em>To search for&nbsp;<strong>RawTX</strong>&nbsp;vulnerability , as a threat prevention for your own&nbsp;<strong>Bitcoin</strong>&nbsp;and&nbsp;<strong>Ethereum</strong>&nbsp;cryptocurrency wallet , we can use and apply various machine learning methods on examples</em>&nbsp;.</p>
</blockquote>



<p>Let’s use the list from&nbsp;&nbsp;<strong><a href="https://dockeyhunt.com/dockeyhunt-deep-learning" target="_blank" rel="noreferrer noopener">“Dockeyhunt Deep Learning”</a></strong>&nbsp;&nbsp;a widely used category of artificial intelligence for business introduction in various fields of cryptanalysis and cryptography in general.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-41-1024x565.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5314"><figcaption class="wp-element-caption"><strong><a href="https://dockeyhunt.com/dockeyhunt-deep-learning" target="_blank" rel="noreferrer noopener">Dockeyhunt Deep Learning</a></strong></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><a href="https://bitcoinchatgpt.org/" target="_blank" rel="noreferrer noopener"><strong>BitcoinChatGPT</strong></a>&nbsp;&nbsp;is an innovative AI-powered chatbot that helps users find vulnerabilities in Bitcoin cryptocurrency transactions. The advantages and classifications of BitcoinChatGPT give you the opportunity to check your Bitcoin address for various crypto wallet attack schemes. Machine learning based on cryptanalysis gives us the full ability to investigate various attacks on the algorithms used in the Bitcoin ecosystem. Tools for extracting private key from the Bitcoin Wallet ledger are widely popular, where BitcoinChatGPT serves as an important and useful resource for cybersecurity.</p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center">Raw Transaction Creation Using BitcoinChatGPT Machine Learning Process</h2>



<p><strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/RawTX.txt" target="_blank" rel="noreferrer noopener">Let’s consider the construction of a vulnerable Raw</a></strong>&nbsp;transaction structure&nbsp;&nbsp;&nbsp;using the&nbsp;&nbsp;<strong><a href="https://bitcoinchatgpt.org/" target="_blank" rel="noreferrer noopener">BitcoinChatGPT</a></strong>&nbsp;module . As an example, let’s take the Bitcoin wallet address:&nbsp;&nbsp;<strong><a href="https://btc1.trezor.io/address/1MjGyKiRLzq4WeuJKyFZMmkjAv7rH1TABm" target="_blank" rel="noreferrer noopener">1MjGyKiRLzq4WeuJKyFZMmkjAv7rH1TABm</a></strong>&nbsp;&nbsp;for the amount of:&nbsp;&nbsp;<strong><a href="https://btc1.trezor.io/address/1MjGyKiRLzq4WeuJKyFZMmkjAv7rH1TABm" target="_blank" rel="noreferrer noopener">131.59300888 BTC</a></strong>&nbsp;&nbsp;and get&nbsp;<code><strong>HASH</strong></code>the public key. Then, using&nbsp;&nbsp;<strong>BitcoinChatGPT</strong>&nbsp;, we will create a vulnerability in Raw transactions, which will allow us to analyze and manipulate the signature data of the ECDSA algorithm.&nbsp;</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>Let’s get&nbsp;<code><strong>HASH</strong></code> the public key using the Python script:&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/wif_to_hash160.py" target="_blank" rel="noreferrer noopener">wif_to_hash160.py</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>To implement&nbsp;<strong><a href="https://polynonce.ru/pip-install-base58/" target="_blank" rel="noreferrer noopener">Base58</a></strong>&nbsp;decoding , install the package:</p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-ebbfd5caf2a2f5718b77459fec78801e" style="color:#4092c2"><code><strong>!pip3 install base58</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-2a7a26deb177a8f63e32f20654d66225" style="color:#4092c2"><code><strong>import base58

def generate_response(input_text):
    input_ids = tokenizer.encode(input_text, return_tensors='pt').cpu()
    response_ids = model.generate(input_ids)
    response_text = tokenizer.decode(response_ids[:, input_ids.shape[-1]:][0], skip_special_tokens=True)
    return response_text

def decode_base58(address):
    decoded = base58.b58decode(address)
    return decoded[1:-4]

if __name__ == "__main__":
    address = input("Enter Bitcoin address:  ")
    decoded_bytes = decode_base58(address)
    print("Bitcoin HASH160: ", decoded_bytes.hex())
    </strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-42-1024x589.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5321"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong>Let’s launch BitcoinChatGPT</strong></p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-319169cb3475b6b0f9b12607f7b63975" style="color:#4092c2"><code><strong>%run BitcoinChatGPT</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code"><code>How to create a vulnerable transaction in Bitcoin for the hashed version of the public key Bitcoin HASH160: <strong>e361516c3163a3d997d7b270c4378816a86343de</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-44-1024x643.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5326"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-874bd875e73b4b464019f6e330d75340" style="color:#4092c2"><code><strong>State of a vulnerable transaction in Bitcoin:

01000000
....01
........0dbc696374c8d7ca61f32710e03aaedcb7a4f2428074814d0e1f4f7f5c1e5935
............00000000
........8b483045
....0221
...........00
...........aafe80d17b0d30de09cbe39a85514aaae0a388135987ab80207e1eed3c915280
....0220
........0d46fb28a4b30599d33325aa8b7633dd0f584f8125bb2e136c88a3e91a6f4238
.....0141
.....04ea7c9e85d4fb089e0b2901cd5c77f3149aa4cf711ed29a3318a4e153a67ea9cd1a22c24c8e05b66eb122db74d26fddf2cb184033fb586743ea330e15eeb8240c
....ffffffff
01
....d204000000000000
........1976
............a914
........e361516c3163a3d997d7b270c4378816a86343de
....88ac
00000000</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p><strong>Let’s combine all the output values ​​into one common string using the Python script&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/combinex.py" target="_blank" rel="noreferrer noopener">combinex.py</a>&nbsp;:</strong></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-45-1024x681.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5327"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<p>The result is a vulnerable transaction.&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/RawTX.txt" target="_blank" rel="noreferrer noopener">RawTX</a></strong>&nbsp;as we know in the context of the Bitcoin blockchain refers to the raw transaction data that is stored on the blockchain in the form of double hashing. This means that&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/RawTX.txt" target="_blank" rel="noreferrer noopener">RawTX</a></strong>&nbsp;is run&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/DoubleSHA256Hasher.py">through the SHA256 algorithm twice</a>&nbsp;to produce the transaction hash that is visible on the blockchain. This hash is known as&nbsp;&nbsp;<a href="https://btc1.trezor.io/address/1MjGyKiRLzq4WeuJKyFZMmkjAv7rH1TABm"><strong>the txid&nbsp;</strong>&nbsp;<em>(transaction identifier)</em></a>&nbsp;.</p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-6db8db9fbec30f8f337c6b1e31dd6bd2" style="color:#4092c2"><code><strong>01000000010dbc696374c8d7ca61f32710e03aaedcb7a4f2428074814d0e1f4f7f5c1e5935000000008b483045022100aafe80d17b0d30de09cbe39a85514aaae0a388135987ab80207e1eed3c91528002200d46fb28a4b30599d33325aa8b7633dd0f584f8125bb2e136c88a3e91a6f4238014104ea7c9e85d4fb089e0b2901cd5c77f3149aa4cf711ed29a3318a4e153a67ea9cd1a22c24c8e05b66eb122db74d26fddf2cb184033fb586743ea330e15eeb8240cffffffff01d2040000000000001976a914e361516c3163a3d997d7b270c4378816a86343de88ac00000000</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h3 class="wp-block-heading has-text-align-center">The process of compromising the extraction of the secret key Nonce value K</h3>



<p><strong>Let’s launch BitcoinChatGPT</strong></p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-319169cb3475b6b0f9b12607f7b63975" style="color:#4092c2"><code><strong>%run BitcoinChatGPT</strong></code></pre>



<pre class="wp-block-code"><code>How a vulnerable RawTX transaction in the Bitcoin blockchain can be compromised to extract the secret key Nonce value K using mathematical methods</code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-46-1024x361.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5333"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center"><a href="https://dustattack.org/blockchain-folbit-leaks" target="_blank" rel="noreferrer noopener">BLOCKCHAIN ​​FOLBIT LEAKS</a></h2>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size">Decode a vulnerable&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/RawTX.txt">RawTX</a></strong>&nbsp;transaction using the&nbsp;<a href="https://dustattack.org/blockchain-folbit-leaks" target="_blank" rel="noreferrer noopener">BLOCKCHAIN ​​FOLBIT LEAKS service function</a></p>
</blockquote>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-53-1024x797.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5347"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size">Result is the value&nbsp;<strong><a href="https://keyhunters.ru/what-is-the-nonce-value-k-in-the-bitcoin-blockchain/" target="_blank" rel="noreferrer noopener">K</a></strong>&nbsp;of the secret key&nbsp;<strong><a href="https://keyhunters.ru/what-is-the-nonce-value-k-in-the-bitcoin-blockchain/" target="_blank" rel="noreferrer noopener">Nonce</a></strong>&nbsp;in&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/calculate.py" target="_blank" rel="noreferrer noopener">HEX format</a></strong></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-7ef15989627c1459e838b8d230c62d64" style="color:#4092c2"><code><strong>K = 39588951cd20e38a6dc86d6b436da7abd2bcad84af3dd16b6f8a83c946c1d3c6</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size">To obtain all other values ​​from the vulnerable&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/RawTX.txt">RawTX</a></strong>&nbsp;transaction, we will use&nbsp;<strong><a href="https://dustattack.org/RSZ-Signature-Decoder" target="_blank" rel="noreferrer noopener">the RSZ Signature Decoder service.</a></strong></p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-54-1024x393.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5356"><figcaption class="wp-element-caption"><strong><a href="https://dustattack.org/RSZ-Signature-Decoder" target="_blank" rel="noreferrer noopener">RSZ Signature Decoder</a></strong></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size">Result values ​​for&nbsp;<strong><a href="https://dustattack.org/RSZ-Signature-Decoder/" target="_blank" rel="noreferrer noopener">R, S, Z</a></strong>&nbsp;in&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/calculate.py" target="_blank" rel="noreferrer noopener">HEX format</a></strong></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-db97338f62bfab2f330ac1ab033f0054" style="color:#4092c2"><code><strong>R = aafe80d17b0d30de09cbe39a85514aaae0a388135987ab80207e1eed3c915280
S = 0d46fb28a4b30599d33325aa8b7633dd0f584f8125bb2e136c88a3e91a6f4238
Z = bbfd05c3355957cbdf44d283b9199eb9741f775a16081288187a82f544fac11f</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>To get the value&nbsp;<strong>X</strong>&nbsp;of the private key from the formula:&nbsp;<code>priv_key = ((((S * K) - Z) * modinv(R, N)) % N)</code>we will use the software&nbsp;<strong><a href="https://dockeyhunt.com/dockeyhunt-private-key-calculator" target="_blank" rel="noreferrer noopener">Dockeyhunt Private Key Calculator</a></strong></p>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-55-1024x615.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5359"><figcaption class="wp-element-caption"><strong><a href="https://dockeyhunt.com/dockeyhunt-private-key-calculator" target="_blank" rel="noreferrer noopener">Dockeyhunt Private Key Calculator</a></strong></figcaption></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size">As a result, we get the value&nbsp;<strong>X</strong>&nbsp;private key in&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/calculate.py" target="_blank" rel="noreferrer noopener">HEX format</a></strong></p>
</blockquote>



<pre class="wp-block-code has-text-color has-link-color wp-elements-eb7aa7b044c6bfa000609cabce1e6fa8" style="color:#4092c2"><code><strong>X = 0x38717b5161c2e817020a0933e1836dd0127bdef59732d77daca20ccfbf61a7ae</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center">Let’s check the obtained private key result using machine learning</h2>



<p><strong>Let’s launch BitcoinChatGPT</strong></p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-319169cb3475b6b0f9b12607f7b63975" style="color:#4092c2"><code><strong>%run BitcoinChatGPT</strong></code></pre>



<pre class="wp-block-code"><code>Apply the BLOCKCHAIN FOLBIT LEAKS function to extract the private key from a vulnerable RawTX transaction in the Bitcoin cryptocurrency
</code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-50-1024x626.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5337"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p class="has-medium-font-size">Finally, the&nbsp;<strong>BitcoinChatGPT</strong>&nbsp;module outputs the response to the file:&nbsp;<strong><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/KEYFOUND.privkey" target="_blank" rel="noreferrer noopener">KEYFOUND.privkey</a></strong>&nbsp;storing the private key in two most used formats&nbsp;<strong>HEX &amp; WIF</strong></p>
</blockquote>



<p><a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/KEYFOUND.privkey">https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/KEYFOUND.privkey</a></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<pre class="wp-block-code has-text-color has-link-color wp-elements-ebbf1852ead19149c51b303429a376ca" style="color:#4092c2"><code><strong>============================= KEYFOUND.privkey =============================

Private Key HEX: 0x38717b5161c2e817020a0933e1836dd0127bdef59732d77daca20ccfbf61a7ae

Private Key WIF: 5JF9ME7zdGLDd3oyuMG7RfwgA1ByjZb2LbSwRMwM8ZKBADFLfCx

Bitcoin Address: 1MjGyKiRLzq4WeuJKyFZMmkjAv7rH1TABm

Balance: 131.59300888 BTC

============================= KEYFOUND.privkey =============================</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>To implement the code, we will install the&nbsp;<strong><a href="https://polynonce.ru/pip-install-bitcoin/" target="_blank" rel="noreferrer noopener">Bitcoin</a></strong>&nbsp;package . This library allows you to create wallets, interact with the blockchain, create and sign transactions, and work with various address formats and private keys of the Bitcoin cryptocurrency.</p>



<pre class="wp-block-code has-text-color has-link-color wp-elements-9a0f1a67ae8617004ae12ce64ce4a4b7" style="color:#4092c2"><code><strong>!pip3 install bitcoin</strong></code></pre>



<hr class="wp-block-separator has-alpha-channel-opacity">



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>Let’s run&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools/blob/main/38QuantumAttacks/priv_addr.py" target="_blank" rel="noreferrer noopener"><strong>the code</strong></a>&nbsp;&nbsp;to check the Bitcoin Address match:</p>
</blockquote>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-51-1024x816.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5338"></figure></div>


<pre class="wp-block-code has-text-color has-link-color wp-elements-1b0d0f4cb5117b9e4bcd853d8d6cb589" style="color:#4092c2"><code><strong>__________________________________________________

Private Key WIF: 38717b5161c2e817020a0933e1836dd0127bdef59732d77daca20ccfbf61a7ae
Bitcoin Address: 1MjGyKiRLzq4WeuJKyFZMmkjAv7rH1TABm
total_received 	= 131.59300888 Bitcoin
__________________________________________________</strong></code></pre>



<p class="has-text-color has-link-color wp-elements-7ce4e2de34bf11d614b363cfa603f081" style="color:#2f8745;font-size:25px"><strong>That’s right! The private key corresponds to the Bitcoin Wallet.</strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading">Let’s open&nbsp;&nbsp;<strong><a href="https://cryptodeeptech.ru/bitaddress.html" target="_blank" rel="noreferrer noopener">bitaddress</a></strong>&nbsp;&nbsp;and check:</h2>



<pre class="wp-block-code has-text-color has-link-color wp-elements-b5a7c266506661691955351ebe0cb73a" style="color:#4092c2"><code><strong>ADDR: 1MjGyKiRLzq4WeuJKyFZMmkjAv7rH1TABm
WIF:  5JF9ME7zdGLDd3oyuMG7RfwgA1ByjZb2LbSwRMwM8ZKBADFLfCx
HEX:  38717b5161c2e817020a0933e1836dd0127bdef59732d77daca20ccfbf61a7ae</strong></code></pre>


<div class="wp-block-image">
<figure class="aligncenter"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-52.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5339"></figure></div>


<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading has-text-align-center">Conclusion and actions to reduce the risk.</h2>



<p>In this article, we explored methods to recover lost cryptocurrency wallets and private keys using mathematical algorithms such as the&nbsp;<a href="https://cryptodeeptech.ru/discrete-logarithm">discrete logarithm</a>&nbsp;and hidden number problems, as well as&nbsp;<strong><a href="https://dustattack.org/blockchain-folbit-leaks">the BLOCKCHAIN ​​FOLBIT LEAKS</a></strong>&nbsp;data leak . We demonstrated how to use software to extract private keys from vulnerable transactions, showing that even secure systems such as Bitcoin have vulnerabilities that can be exploited to regain access to lost funds.</p>



<p>To protect against threats related to the Bitcoin cryptocurrency transaction RawTX vulnerability, users should take the following steps:</p>



<ol class="wp-block-list">
<li><strong>Software Updates</strong>&nbsp;: Regularly updating your cryptocurrency wallets to patched versions is critical to security.</li>



<li><strong>Improved signature verification mechanisms</strong>&nbsp;: Stronger input validation and error handling will help prevent the creation of fake signatures and protect users’ private keys.</li>



<li><strong>Network activity monitoring</strong>&nbsp;: Constant analysis of network status and early detection of suspicious transactions allow for prompt response to attempts to exploit vulnerabilities.</li>



<li><strong>Implementing Multi-Factor Authentication</strong>&nbsp;: Implementing additional cryptographic protection methods will significantly improve security.</li>
</ol>



<blockquote class="wp-block-quote is-layout-flow wp-block-quote-is-layout-flow">
<p>To protect against potential attacks related to the RawTX vulnerability in Bitcoin transactions, users are advised to update their wallet software to the latest versions. Regular updates, the use of anomaly monitoring systems, and increasing user awareness of potential threats will help maintain the security and integrity of cryptocurrency systems.</p>
</blockquote>



<p>The RawTX vulnerability in Bitcoin transactions poses a serious threat to the security of cryptocurrency transactions and the integrity of the blockchain. To mitigate the risks, users should regularly update their software, implement strict security measures, and constantly monitor the state of the network. These actions will help maintain the security and stability of cryptocurrency systems, protecting users from potential attacks and financial losses.</p>



<p>Our study shows the importance of mathematical analysis in cryptocurrencies and demonstrates the potential of using complex mathematical methods to solve practical problems in cryptanalysis. However, these methods can be applied both to restore access to lost funds and to exploit vulnerabilities, which highlights the need to strengthen the security of cryptocurrency systems.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<h2 class="wp-block-heading">References:</h2>



<ol class="wp-block-list">
<li><em><strong><a href="https://cryptodeeptech.ru/doc/Analyzing_Quantum_Vulnerabilities_The_Insecurity_of_Classical_Proof_Systems_in_Quantum_Contexts.pdf" target="_blank" rel="noreferrer noopener">Analyzing Quantum Vulnerabilities:</a></strong>&nbsp;The Insecurity of Classical Proof Systems in Quantum Contexts</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Enhancing_Security_The_Impact_of_Iteration_on_Quantum_Attacks_Against_Block_Ciphers.pdf" target="_blank" rel="noreferrer noopener">Enhancing Security:</a></strong>&nbsp;The Impact of Iteration on Quantum Attacks Against Block Ciphers</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Assessing_Quantum_Threats_to_Bitcoin_Risks_and_Protective_Strategies_for_Cryptocurrencies.pdf" target="_blank" rel="noreferrer noopener">Assessing Quantum Threats to Bitcoin:</a></strong>&nbsp;Risks and Protective Strategies for Cryptocurrencies</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Quantum_Threats_to_Pseudorandom_Generators_Analyzing_Attacks_on_the_Blum-Micali_Generator.pdf" target="_blank" rel="noreferrer noopener">Quantum Threats to Pseudorandom Generators:</a></strong>&nbsp;Analyzing Attacks on the Blum-Micali Generator</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Advancing_Quantum_Collision_Attacks_Analyzing_SHA-256_and_SHA-512_Vulnerabilities.pdf" target="_blank" rel="noreferrer noopener">Advancing Quantum Collision Attacks:</a></strong>&nbsp;Analyzing SHA-256 and SHA-512 Vulnerabilities</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Exploring_Quantum_Vulnerabilities_Attacks_on_Beyond-Birthday-Bound_MACs.pdf" target="_blank" rel="noreferrer noopener">Exploring Quantum Vulnerabilities:</a></strong>&nbsp;Attacks on Beyond-Birthday-Bound MAC’s</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Enhancing_Quantum_Cybersecurity_Advanced_Variational_Attacks_on_Cryptographic_Protocols.pdf" target="_blank" rel="noreferrer noopener">Enhancing Quantum Cybersecurity:</a></strong>&nbsp;Advanced Variational Attacks on Cryptographic Protocols</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Exploring_Practical_Quantum_Cryptography_Capabilities_Implementations_and_Attack_Vulnerabilities.pdf" target="_blank" rel="noreferrer noopener">Exploring Practical Quantum Cryptography:</a></strong>&nbsp;Capabilities, Implementations, and Attack Vulnerabilities</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Navigating_the_Shift_to_Quantum_Resistance_Preparing_for_the_Future_of_Cryptography.pdf" target="_blank" rel="noreferrer noopener">Navigating the Shift to Quantum Resistance:</a></strong>&nbsp;Preparing for the Future of Cryptography</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Securing_the_Quantum_Age_Exploring_Quantum-Resistant_Cryptographic_Protocols.pdf" target="_blank" rel="noreferrer noopener">Securing the Quantum Age:</a></strong>&nbsp;Exploring Quantum-Resistant Cryptographic Protocols</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Quantum-Resistant_Code-Based_Cryptosystem_A_Novel_Approach_Using_Repetition_of_Error-Correcting_Codes.pdf" target="_blank" rel="noreferrer noopener">Quantum-Resistant Code-Based Cryptosystem:</a></strong>&nbsp;A Novel Approach Using Repetition of Error-Correcting Codes</em></li>



<li><em><a href="https://cryptodeeptech.ru/doc/Assessing_Electromagnetic_Side-Channel_Attack_Risks_in_Quantum_Key_Distribution_Receivers_Using_Multi-Class_Classification.pdf" target="_blank" rel="noreferrer noopener"><strong>Assessing Electromagnetic Side-Channel Attack Risks</strong></a>&nbsp;in Quantum Key Distribution Receivers Using Multi-Class Classification</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Managing_Cryptographic_and_Quantum_Risks_A_Practical_Guide_for_Organizations.pdf" target="_blank" rel="noreferrer noopener">Managing Cryptographic and Quantum Risks:</a></strong>&nbsp;A Practical Guide for Organizations</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Enhancing_Cloud_Security_Quantum_Cryptography_Algorithms_for_Robust_Data_Storage_and_Processing.pdf" target="_blank" rel="noreferrer noopener">Enhancing Cloud Security:</a></strong>&nbsp;Quantum Cryptography Algorithms for Robust Data Storage and Processing</em></li>



<li><strong><em><a href="https://cryptodeeptech.ru/doc/Transitioning_to_Quantum-Safe_Cryptography_on_IBM_Z_A_Guide_for_Secure_Data_Protection.pdf" target="_blank" rel="noreferrer noopener">Transitioning to Quantum-Safe Cryptography on IBM Z:</a></em></strong>&nbsp;<em>A Guide for Secure Data Protection</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Post-Quantum_Attacks_on_Symmetric-Key_Cryptography_Analyzing_Vulnerabilities_and_Defense_Strategies.pdf" target="_blank" rel="noreferrer noopener">Post-Quantum Attacks on Symmetric-Key Cryptography:</a></strong>&nbsp;Analyzing Vulnerabilities and Defense Strategies</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Report_on_Post-Quantum_Cryptography_NIST_Strategies_for_Securing_Digital_Communications_Against_Quantum_Threats.pdf" target="_blank" rel="noreferrer noopener">Report on Post-Quantum Cryptography:</a>&nbsp;</strong>NIST’s Strategies for Securing Digital Communications Against Quantum Threats</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Quantum_Computing_and_Cybersecurity_Navigating_Emerging_Threats_and_Mitigation_Strategies.pdf" target="_blank" rel="noreferrer noopener">Quantum Computing and Cybersecurity:</a></strong>&nbsp;Navigating Emerging Threats and Mitigation Strategies</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Revolutionizing_Currency_The_Concept_and_Development_of_Quantum_Money.pdf" target="_blank" rel="noreferrer noopener">Revolutionizing Currency:</a></strong>&nbsp;The Concept and Development of Quantum Money</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Post-Quantum_Cryptography_Preparing_for_Quantum_Threats_and_Securing_the_Future_of_Encryption.pdf" target="_blank" rel="noreferrer noopener">Post-Quantum Cryptography:</a></strong>&nbsp;Preparing for Quantum Threats and Securing the Future of Encryption</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Ensuring_Digital_Sovereignty_The_Critical_Role_of_Cryptographic_Security_in_Europe.pdf" target="_blank" rel="noreferrer noopener">Ensuring Digital Sovereignty:</a></strong>&nbsp;The Critical Role of Cryptographic Security in Europe</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Preparing_for_the_Quantum_Threat_Safeguarding_Sensitive_Information_Against_Future_Risks.pdf" target="_blank" rel="noreferrer noopener">Preparing for the Quantum Threat:</a></strong>&nbsp;Safeguarding Sensitive Information Against Future Risks</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Defending_Quantum_Private_Communication_Strategies_Against_Trojan_Horse_Attacks.pdf" target="_blank" rel="noreferrer noopener">Defending Quantum Private Communication:</a></strong>&nbsp;Strategies Against Trojan Horse Attacks</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Bitcoins_Quantum_Resistance_A_Commit-Delay-Reveal_Protocol_for_Secure_Transition.pdf" target="_blank" rel="noreferrer noopener">Bitcoin’s Quantum Resistance:</a></strong>&nbsp;A Commit-Delay-Reveal Protocol for Secure Transition</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Project_Leap_Safeguarding_the_Financial_System_in_the_Quantum_Era.pdf" target="_blank" rel="noreferrer noopener">Project Leap:</a></strong>&nbsp;Safeguarding the Financial System in the Quantum Era</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Quantum_Threats_to_Bitcoin_Vulnerabilities_and_Mitigation_Strategies.pdf" target="_blank" rel="noreferrer noopener">Quantum Threats to Bitcoin:</a></strong>&nbsp;Vulnerabilities and Mitigation Strategies</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Navigating_the_Quantum_Frontier_Understanding_Quantum_Computing_and_the_Rise_of_Post-Quantum_Cryptography.pdf" target="_blank" rel="noreferrer noopener">Navigating the Quantum Frontier:</a></strong>&nbsp;Understanding Quantum Computing and the Rise of Post-Quantum Cryptography</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Quantum_Origin_Revolutionizing_Cryptographic_Key_Generation_with_Verifiable_Quantum_Randomness.pdf" target="_blank" rel="noreferrer noopener">Quantum Origin:</a></strong>&nbsp;Revolutionizing Cryptographic Key Generation with Verifiable Quantum Randomness</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/Developing_Quantum-Resistant_Cryptography_Encryption_for_a_Post-Quantum_World.pdf" target="_blank" rel="noreferrer noopener">Developing Quantum-Resistant Cryptography:</a></strong>&nbsp;Encryption for a Post-Quantum World</em></li>



<li><strong><em><a href="https://cryptodeeptech.ru/doc/Quantum-Safe_Cryptography_Addressing_the_Challenges_and_Opportunities_in_a_Quantum_Computing_Era.pdf" target="_blank" rel="noreferrer noopener">Quantum-Safe Cryptography:</a></em></strong>&nbsp;<em>Addressing the Challenges and Opportunities in a Quantum Computing Era</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/The_Quantum_Computing_Revolution_Implications_for_Modern_Cryptographic_Security.pdf" target="_blank" rel="noreferrer noopener">The Quantum Computing Revolution:</a></strong>&nbsp;Implications for Modern Cryptographic Security</em></li>



<li><strong><a href="https://cryptodeeptech.ru/doc/Private-Key_Public-Key_Cryptography_in_the_Quantum_Era_Security_Risks_and_Future_Strategies.pdf" target="_blank" rel="noreferrer noopener"><em>Private-Key</em>&nbsp;&amp;&nbsp;<em>Public-Key Cryptography in the Quantum Era:</em></a></strong><em>&nbsp;Security Risks and Future Strategies</em></li>



<li><em><strong><a href="https://cryptodeeptech.ru/doc/The_Quantum_Risk_Paradox_Why_the_Threat_Is_Already_Here.pdf" target="_blank" rel="noreferrer noopener">The Quantum Risk Paradox:</a></strong>&nbsp;Why the Threat Is Already Here</em>&nbsp;<em>(Quantum Threat Timeline)</em></li>
</ol>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p></p>


<div class="wp-block-image">
<figure class="aligncenter size-full is-resized"><a href="https://dzen.ru/video/watch/67c3e91abbfa683a745a0aea"><img loading="lazy" decoding="async" width="670" height="390" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/image-8(1).png" alt="Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats" class="wp-image-3249" style="width:830px;height:auto" srcset="https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-8.png 670w, https://cryptodeeptech.ru/wp-content/uploads/2025/03/image-8-300x175.png 300w" sizes="auto, (max-width: 670px) 100vw, 670px"></a></figure></div>


<p></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p>This material was created for the&nbsp;&nbsp;<a href="https://cryptodeep.ru/" target="_blank" rel="noreferrer noopener">CRYPTO DEEP TECH</a>&nbsp;portal &nbsp;to ensure financial data security and cryptography on elliptic curves&nbsp;&nbsp;<a href="https://www.youtube.com/@cryptodeeptech" target="_blank" rel="noreferrer noopener">secp256k1</a>&nbsp;&nbsp;against weak&nbsp;&nbsp;<a href="https://github.com/demining/CryptoDeepTools" target="_blank" rel="noreferrer noopener">ECDSA</a>&nbsp;signatures &nbsp;in the&nbsp;&nbsp;<a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener">BITCOIN</a>&nbsp;cryptocurrency . The creators of the software are not responsible for the use of materials.</p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p><strong><a href="https://github.com/demining/CryptoDeepTools/tree/main/38QuantumAttacks" target="_blank" rel="noreferrer noopener">Source code</a></strong></p>



<p><strong><a href="https://colab.research.google.com/drive/1jqHX5Oawy3QPh2OSYVf6AF1RGtjAb4rj?usp=sharing" target="_blank" rel="noreferrer noopener">Google Colab</a></strong></p>



<p><strong><a href="https://bitcoinchatgpt.org/" target="_blank" rel="noreferrer noopener">BitcoinChatGPT</a></strong></p>



<p><strong><a href="https://dustattack.org/blockchain-folbit-leaks" target="_blank" rel="noreferrer noopener">Blockchain Folbit Leaks</a></strong></p>



<p><strong><a href="https://dockeyhunt.com/dockeyhunt-deep-learning" target="_blank" rel="noreferrer noopener">Dockeyhunt Deep Learning</a></strong></p>



<p><strong><a href="https://t.me/cryptodeeptech" target="_blank" rel="noreferrer noopener">Telegram: https://t.me/cryptodeeptech</a></strong></p>



<p><strong><a href="https://youtu.be/p62orC7WDUE" target="_blank" rel="noreferrer noopener">Video material: https://youtu.be/p62orC7WDUE</a></strong></p>



<p><strong><a href="https://dzen.ru/video/watch/67c3e91abbfa683a745a0aea" target="_blank" rel="noreferrer noopener">Video tutorial: https://dzen.ru/video/watch/67c3e91abbfa683a745a0aea</a></strong></p>



<p><strong><a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin" target="_blank" rel="noreferrer noopener">Source: https://cryptodeeptech.ru/quantum-attacks-on-bitcoin</a></strong></p>



<hr class="wp-block-separator has-alpha-channel-opacity">



<figure class="wp-block-image"><img decoding="async" src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/060-1-1024x576.png" alt="Quantum Attacks on Bitcoin: Vulnerability Assessment and Defense Strategies Against New Quantum Computing Threats" class="wp-image-5301"></figure>



<hr class="wp-block-separator has-alpha-channel-opacity">



<p></p>
	</div><!-- .entry-content -->

	<footer class="entry-footer">
		<div class="cat-links"><i class="fa fa-folder-open" aria-hidden="true"></i> <a href="https://cryptodeeptech.ru/category/cryptanalysis/" rel="category tag">Cryptanalysis</a></div><div class="edit-link"><a class="post-edit-link" href="https://cryptodeeptech.ru/wp-admin/post.php?post=3236&amp;action=edit">Edit <span class="screen-reader-text">Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats</span></a></div>	</footer><!-- .entry-footer -->
</article><!-- #post-3236 -->

	<nav class="navigation post-navigation" aria-label="Posts">
		<h2 class="screen-reader-text">Post navigation</h2>
		<div class="nav-links"><div class="nav-previous"><a href="https://cryptodeeptech.ru/quantum-attacks-on-bitcoin/" rel="prev">Quantum Attacks on Bitcoin: Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats</a></div></div>
	</nav>		<div id="itng_related_posts_wrapper">
			<h3 id="itng_related_posts_title">Related Posts</h3>
			<div class="itng-related-posts row">
				<article id="post-2321" class="itng-blog col-md-6 col-lg-4 post-2321 post type-post status-publish format-standard hentry category-cryptanalysis">
		<div class="itng-card-wrapper">
			<div class="itng-thumb">
							</div>
			
			<div class="itng-card-content">
				<div class="entry-meta">
					<a href="https://cryptodeeptech.ru/dao-exploit/"></a>
					<span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>				</div><!-- .entry-meta -->
				
				<header class="entry-header">
					<h2 class="entry-title"><a href="https://cryptodeeptech.ru/dao-exploit/">Cryptanalysis of the DAO exploit &amp; Multi-Stage Attack</a></h2>				</header><!-- .entry-header -->
				
				<div class="itng_excerpt">
					In this article, we will look at a bug in the DAO code. The hacker exploited a bug in the code of the DAO and stole more or less $50 million worth of ether. I will focus here only on the main technical issue of the exploit: The fallback function. For a more detailed and advanced recount…				</div>
				
				<div class="blog-footer">
					<div class="itng_cats">
						<a href="https://cryptodeeptech.ru/category/cryptanalysis/" rel="category tag">Cryptanalysis</a>					</div>
					<div class="blog-comments">
						0					</div>
				</div>
			</div>
		</div>
</article><!-- #post-2321 --><article id="post-1219" class="itng-blog col-md-6 col-lg-4 post-1219 post type-post status-publish format-standard hentry category-cryptanalysis">
		<div class="itng-card-wrapper">
			<div class="itng-thumb">
							</div>
			
			<div class="itng-card-content">
				<div class="entry-meta">
					<a href="https://cryptodeeptech.ru/defi-attacks/"></a>
					<span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>				</div><!-- .entry-meta -->
				
				<header class="entry-header">
					<h2 class="entry-title"><a href="https://cryptodeeptech.ru/defi-attacks/">DeFi Attacks &amp; Exploits all the biggest cryptocurrency thefts from 2021 to 2022</a></h2>				</header><!-- .entry-header -->
				
				<div class="itng_excerpt">
					In this article, we will tell you about the most daring and biggest thefts of cryptocurrencies associated with&nbsp;платформой DeFi.&nbsp;Hackers had a big year in 2021 when they stole $3.2 billion worth of cryptocurrencies.&nbsp;But in 2022, the amount of theft of cryptocurrencies reached a historical maximum.&nbsp;In the first three months of this year, hackers have stolen $1.3 billion&nbsp;from…				</div>
				
				<div class="blog-footer">
					<div class="itng_cats">
						<a href="https://cryptodeeptech.ru/category/cryptanalysis/" rel="category tag">Cryptanalysis</a>					</div>
					<div class="blog-comments">
						0					</div>
				</div>
			</div>
		</div>
</article><!-- #post-1219 --><article id="post-1719" class="itng-blog col-md-6 col-lg-4 post-1719 post type-post status-private format-standard hentry category-cryptanalysis">
		<div class="itng-card-wrapper">
			<div class="itng-thumb">
							</div>
			
			<div class="itng-card-content">
				<div class="entry-meta">
					<a href="https://cryptodeeptech.ru/vulnerabilities-3-state-variable-default-visibility/"></a>
					<span class="byline"> <span class="author vcard"><a class="url fn n" href="https://cryptodeeptech.ru/author/cryptodeeptech/">Crypto Deep Tech</a></span></span>				</div><!-- .entry-meta -->
				
				<header class="entry-header">
					<h2 class="entry-title"><a href="https://cryptodeeptech.ru/vulnerabilities-3-state-variable-default-visibility/">Private: Vulnerabilities 3 State Variable Default Visibility</a></h2>				</header><!-- .entry-header -->
				
				<div class="itng_excerpt">
					State Variable Default Visibility It's common for developers to explicitly declare function visibility, but not so common to declare variable visibility. State variables can have one of three visibility identifiers:&nbsp;public,&nbsp;internal, or&nbsp;private. Luckily, the default visibility for variables is internal and not public, but even if you intend on declaring a variable as internal, it's important to be…				</div>
				
				<div class="blog-footer">
					<div class="itng_cats">
						<a href="https://cryptodeeptech.ru/category/cryptanalysis/" rel="category tag">Cryptanalysis</a>					</div>
					<div class="blog-comments">
						0					</div>
				</div>
			</div>
		</div>
</article><!-- #post-1719 -->			</div>
		</div>
			<div id="author_box" class="row no-gutters">
			<div class="author_avatar col-2">
							</div>
			<div class="author_info col-10">
				<h4 class="author_name title-font">
					Crypto Deep Tech				</h4>
				<div class="author_bio">
									</div>
			</div>
		</div>
	
	</main><!-- #main -->

</div><!-- #content-wrapper -->


 <div id="footer-sidebar" class="widget-area">
    <div class="container">
        <div class="row">
                    </div>
    </div>
</div>
	<footer id="colophon" class="site-footer">
		<div class="container">
			<div class="site-info">
				Donation Address: <a href="https://www.blockchain.com/btc/address/1Lw2gTnMpxRUNBU85Hg4ruTwnpUPKdf3nV" target="_blank">♥  BTC: 1Lw2gTnMpxRUNBU85Hg4ruTwnpUPKdf3nV</a>				<span class="sep"> | </span>
					Copyright © 2025 «CRYPTO DEEP TECH». 			</div><!-- .site-info -->
		</div>
	</footer><!-- #colophon -->
</div><!-- #page -->

<nav id="menu" class="panel" role="navigation" style="position: fixed; top: 0px; bottom: 0px; height: 100%; left: -15.625em; width: 15.625em;">
	<div class="menu-overlay"></div>
	<div id="panel-top-bar">
		<button class="go-to-bottom"></button>
		<button id="close-menu" class="menu-link"><i class="fa fa-chevron-left" aria-hidden="true"></i></button>
	</div>

	<ul id="menu-main" class="menu"><li id="menu-item-229" class="menu-item menu-item-type-custom menu-item-object-custom menu-item-home"><a href="https://cryptodeeptech.ru/">HOME</a></li>
<li id="menu-item-225" class="menu-item menu-item-type-post_type menu-item-object-page"><a href="https://cryptodeeptech.ru/publication/">PUBLICATIONS</a></li>
<li id="menu-item-226" class="menu-item menu-item-type-post_type menu-item-object-page"><a href="https://cryptodeeptech.ru/study/">STUDY</a></li>
<li id="menu-item-227" class="menu-item menu-item-type-post_type menu-item-object-page"><a href="https://cryptodeeptech.ru/resources/">RESOURCES</a></li>
<li id="menu-item-228" class="menu-item menu-item-type-post_type menu-item-object-page"><a href="https://cryptodeeptech.ru/contacts/">CONTACTS</a></li>
<li id="menu-item-240" class="menu-item menu-item-type-post_type menu-item-object-post"><a href="https://cryptodeeptech.ru/lattice-attack/">BLOG</a></li>
<li id="menu-item-541" class="menu-item menu-item-type-post_type menu-item-object-page"><a href="https://cryptodeeptech.ru/eng/">ENG</a></li>
<li id="menu-item-542" class="menu-item menu-item-type-post_type menu-item-object-page"><a href="https://cryptodeeptech.ru/rus/">RUS</a></li>
<li id="menu-item-1974" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children"><a href="https://cryptodeeptech.ru/other-languages/">Other Languages</a><span class="dropdown-arrow" tabindex="0"><i class="fa fa-angle-down"></i></span>
<ul class="sub-menu" style="display: none;">
	<li id="menu-item-1975" class="menu-item menu-item-type-post_type menu-item-object-page"><a href="https://cryptodeeptech.ru/cn/">CN</a></li>
	<li id="menu-item-1992" class="menu-item menu-item-type-post_type menu-item-object-page"><a href="https://cryptodeeptech.ru/kr/">KR</a></li>
	<li id="menu-item-2839" class="menu-item menu-item-type-post_type menu-item-object-page"><a href="https://cryptodeeptech.ru/jp/">JP</a></li>
</ul>
</li>
</ul>
	<button class="go-to-top"></button>
</nav>

<div id="sticky-navigation">
	<div class="nav-wrapper">
		 <div class="container">

			 <div class="row justify-content-end align-items-center justify-content-between no-gutters">


				<div class="main-navigation col-lg-9" role="navigation">
					<ul id="menu-desktop" class="menu"><li class="menu-item menu-item-type-custom menu-item-object-custom menu-item-home menu-item-229"><a href="https://cryptodeeptech.ru/">HOME</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-225"><a href="https://cryptodeeptech.ru/publication/">PUBLICATIONS</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-226"><a href="https://cryptodeeptech.ru/study/">STUDY</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-227"><a href="https://cryptodeeptech.ru/resources/">RESOURCES</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-228"><a href="https://cryptodeeptech.ru/contacts/">CONTACTS</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-post menu-item-240"><a href="https://cryptodeeptech.ru/lattice-attack/">BLOG</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-541"><a href="https://cryptodeeptech.ru/eng/">ENG</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-542"><a href="https://cryptodeeptech.ru/rus/">RUS</a></li>
<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children menu-item-1974"><a href="https://cryptodeeptech.ru/other-languages/">Other Languages</a>
<ul class="sub-menu">
	<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-1975"><a href="https://cryptodeeptech.ru/cn/">CN</a></li>
	<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-1992"><a href="https://cryptodeeptech.ru/kr/">KR</a></li>
	<li class="menu-item menu-item-type-post_type menu-item-object-page menu-item-2839"><a href="https://cryptodeeptech.ru/jp/">JP</a></li>
</ul>
</li>
</ul>				</div>

				<button href="#menu" class="menu-link mobile-nav-btn"><i class="fa fa-bars" aria-hidden="true"></i></button>

				<button type="button" id="go-to-field" tabindex="-1"></button>

				<button class="search-btn-sticky ml-auto col-auto"><i class="fa fa-search"></i></button>
				
<div class="itng-search-sticky">
	<form role="search" method="get" class="search-form" action="https://cryptodeeptech.ru/">
				<label>
					<span class="screen-reader-text">Search for:</span>
					<input type="search" class="search-field" placeholder="Search …" value="" name="s">
				</label>
				<input type="submit" class="search-submit" value="Search">
			</form>	<button type="button" id="go-to-btn" tabindex="-1"></button>
</div>

			</div>
		</div>
	</div>
</div>

<div id="itng-back-to-top" class="show"><i class="fa fa-chevron-up" aria-hidden="true"></i></div>

		<script type="text/javascript">
							jQuery("#post-3236 .entry-meta .date").css("display","none");
					jQuery("#post-3236 .entry-date").css("display","none");
					jQuery("#post-3236 .posted-on").css("display","none");
							jQuery("#post-2321 .entry-meta .date").css("display","none");
					jQuery("#post-2321 .entry-date").css("display","none");
					jQuery("#post-2321 .posted-on").css("display","none");
							jQuery("#post-1219 .entry-meta .date").css("display","none");
					jQuery("#post-1219 .entry-date").css("display","none");
					jQuery("#post-1219 .posted-on").css("display","none");
							jQuery("#post-1719 .entry-meta .date").css("display","none");
					jQuery("#post-1719 .entry-date").css("display","none");
					jQuery("#post-1719 .posted-on").css("display","none");
				</script>
				<script type="text/javascript">
				var wpfc_ajaxurl = "https://cryptodeeptech.ru/wp-admin/admin-ajax.php";
				var wpfc_nonce = "1b2d0e42fc";
			</script>
			<style id="core-block-supports-inline-css">
.wp-elements-7ce4e2de34bf11d614b363cfa603f081 a:where(:not(.wp-element-button)){color:#2f8745;}.wp-elements-fa7876f849273a89517e062a3926eb18 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-a6943f49ad156aae464fc8259396a45d a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-460cf49ce80c6a22dd14e4c8aa89db70 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-f7f7757716b43f96a1bee4329b016d7d a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-b4604e3f1fd41580421b53a71ef27a15 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-00d82d61f50918158f2f96a4a33cb9a4 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-ebbfd5caf2a2f5718b77459fec78801e a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-2a7a26deb177a8f63e32f20654d66225 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-319169cb3475b6b0f9b12607f7b63975 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-874bd875e73b4b464019f6e330d75340 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-6db8db9fbec30f8f337c6b1e31dd6bd2 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-7ef15989627c1459e838b8d230c62d64 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-db97338f62bfab2f330ac1ab033f0054 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-eb7aa7b044c6bfa000609cabce1e6fa8 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-ebbf1852ead19149c51b303429a376ca a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-9a0f1a67ae8617004ae12ce64ce4a4b7 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-1b0d0f4cb5117b9e4bcd853d8d6cb589 a:where(:not(.wp-element-button)){color:#4092c2;}.wp-elements-b5a7c266506661691955351ebe0cb73a a:where(:not(.wp-element-button)){color:#4092c2;}
</style>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/hoverintent-js.min.js" id="hoverintent-js-js"></script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/admin-bar.min.js" id="admin-bar-js"></script>
<script id="wp-statistics-tracker-js-extra">
var WP_Statistics_Tracker_Object = {"requestUrl":"https:\/\/cryptodeeptech.ru\/wp-json\/wp-statistics\/v2","ajaxUrl":"https:\/\/cryptodeeptech.ru\/wp-admin\/admin-ajax.php","hitParams":{"wp_statistics_hit":1,"source_type":"post","source_id":3236,"search_query":"","signature":"300c011c5a05f0bc553f33d914e4b5ce","endpoint":"hit"},"onlineParams":{"wp_statistics_hit":1,"source_type":"post","source_id":3236,"search_query":"","signature":"300c011c5a05f0bc553f33d914e4b5ce","endpoint":"online"},"option":{"userOnline":"1","consentLevel":"disabled","dntEnabled":false,"bypassAdBlockers":false,"isWpConsentApiActive":false,"trackAnonymously":false,"isPreview":false},"jsCheckTime":"60000"};
</script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/tracker.js" id="wp-statistics-tracker-js"></script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/chart.umd.min.js" id="wp-statistics-chart.js-js"></script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/mini-chart.js" id="wp-statistics-mini-chart-js"></script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/bigSlide.js" id="big-slide-js"></script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/owl.carousel.js" id="owl-js-js"></script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/jquery.magnific-popup.min.js" id="mag-lightbox-js-js"></script>
<script id="itng-custom-js-js-extra">
var itng = {"toTopEnable":"1","stickyNav":""};
</script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/custom.js" id="itng-custom-js-js"></script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/navigation.js" id="itng-navigation-js"></script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/toolbar.js" id="wpfc-toolbar-js"></script>
<script id="autoptimize-toolbar-js-extra">
var autoptimize_ajax_object = {"ajaxurl":"https:\/\/cryptodeeptech.ru\/wp-admin\/admin-ajax.php","error_msg":"Your Autoptimize cache might not have been purged successfully, please check on the <a href=\"https:\/\/cryptodeeptech.ru\/wp-admin\/options-general.php?page=autoptimize\" style=\"white-space:nowrap;\">Autoptimize settings page<\/a>.","dismiss_msg":"Dismiss this notice.","nonce":"db97598f3f"};
</script>
<script src="./Quantum Attacks on Bitcoin_ Assessing Vulnerabilities and Developing Defense Strategies Against Emerging Quantum Computing Threats - CRYPTO DEEP TECH_files/toolbar.min.js" id="autoptimize-toolbar-js"></script>

<!-- Yandex.Metrika counter -->
<script type="text/javascript">
   (function(m,e,t,r,i,k,a){m[i]=m[i]||function(){(m[i].a=m[i].a||[]).push(arguments)};
   var z = null;m[i].l=1*new Date();
   for (var j = 0; j < document.scripts.length; j++) {if (document.scripts[j].src === r) { return; }}
   k=e.createElement(t),a=e.getElementsByTagName(t)[0],k.async=1,k.src=r,a.parentNode.insertBefore(k,a)})
   (window, document, "script", "https://mc.yandex.ru/metrika/tag.js", "ym");

   ym(89995532, "init", {
        clickmap:true,
        trackLinks:true,
        accurateTrackBounce:true,
        webvisor:true
   });
</script>
<noscript><div><img src="https://mc.yandex.ru/watch/89995532" style="position:absolute; left:-9999px;" alt="" /></div></noscript>
<!-- /Yandex.Metrika counter -->




<div id="revert-loader-toolbar"></div></body></html>
