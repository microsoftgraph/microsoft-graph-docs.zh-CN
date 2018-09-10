# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="f6eca-101">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6eca-101">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="f6eca-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f6eca-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6eca-103">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="f6eca-103">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="f6eca-104">属性</span><span class="sxs-lookup"><span data-stu-id="f6eca-104">Properties</span></span>
|<span data-ttu-id="f6eca-105">属性</span><span class="sxs-lookup"><span data-stu-id="f6eca-105">Property</span></span>|<span data-ttu-id="f6eca-106">类型</span><span class="sxs-lookup"><span data-stu-id="f6eca-106">Type</span></span>|<span data-ttu-id="f6eca-107">说明</span><span class="sxs-lookup"><span data-stu-id="f6eca-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6eca-108">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="f6eca-108">encryptionKey</span></span>|<span data-ttu-id="f6eca-109">Binary</span><span class="sxs-lookup"><span data-stu-id="f6eca-109">Binary</span></span>|<span data-ttu-id="f6eca-110">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="f6eca-110">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="f6eca-111">initializationVector</span><span class="sxs-lookup"><span data-stu-id="f6eca-111">initializationVector</span></span>|<span data-ttu-id="f6eca-112">Binary</span><span class="sxs-lookup"><span data-stu-id="f6eca-112">Binary</span></span>|<span data-ttu-id="f6eca-113">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="f6eca-113">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="f6eca-114">mac</span><span class="sxs-lookup"><span data-stu-id="f6eca-114">mac</span></span>|<span data-ttu-id="f6eca-115">Binary</span><span class="sxs-lookup"><span data-stu-id="f6eca-115">Binary</span></span>|<span data-ttu-id="f6eca-116">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="f6eca-116">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="f6eca-117">macKey</span><span class="sxs-lookup"><span data-stu-id="f6eca-117">macKey</span></span>|<span data-ttu-id="f6eca-118">Binary</span><span class="sxs-lookup"><span data-stu-id="f6eca-118">Binary</span></span>|<span data-ttu-id="f6eca-119">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="f6eca-119">The key used to get mac.</span></span>|
|<span data-ttu-id="f6eca-120">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="f6eca-120">profileIdentifier</span></span>|<span data-ttu-id="f6eca-121">String</span><span class="sxs-lookup"><span data-stu-id="f6eca-121">String</span></span>|<span data-ttu-id="f6eca-122">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="f6eca-122">The the profile identifier.</span></span>|
|<span data-ttu-id="f6eca-123">fileDigest</span><span class="sxs-lookup"><span data-stu-id="f6eca-123">fileDigest</span></span>|<span data-ttu-id="f6eca-124">Binary</span><span class="sxs-lookup"><span data-stu-id="f6eca-124">Binary</span></span>|<span data-ttu-id="f6eca-125">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="f6eca-125">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="f6eca-126">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f6eca-126">fileDigestAlgorithm</span></span>|<span data-ttu-id="f6eca-127">String</span><span class="sxs-lookup"><span data-stu-id="f6eca-127">String</span></span>|<span data-ttu-id="f6eca-128">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="f6eca-128">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6eca-129">关系</span><span class="sxs-lookup"><span data-stu-id="f6eca-129">Relationships</span></span>
<span data-ttu-id="f6eca-130">无</span><span class="sxs-lookup"><span data-stu-id="f6eca-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f6eca-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6eca-131">JSON Representation</span></span>
<span data-ttu-id="f6eca-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6eca-132">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```








