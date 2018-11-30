---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
ms.openlocfilehash: 92aceaa56221287dcde67dcefb4d9ae7109d9273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011061"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="397e5-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="397e5-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="397e5-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="397e5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="397e5-105">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="397e5-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="397e5-106">属性</span><span class="sxs-lookup"><span data-stu-id="397e5-106">Properties</span></span>
|<span data-ttu-id="397e5-107">属性</span><span class="sxs-lookup"><span data-stu-id="397e5-107">Property</span></span>|<span data-ttu-id="397e5-108">类型</span><span class="sxs-lookup"><span data-stu-id="397e5-108">Type</span></span>|<span data-ttu-id="397e5-109">说明</span><span class="sxs-lookup"><span data-stu-id="397e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="397e5-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="397e5-110">encryptionKey</span></span>|<span data-ttu-id="397e5-111">Binary</span><span class="sxs-lookup"><span data-stu-id="397e5-111">Binary</span></span>|<span data-ttu-id="397e5-112">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="397e5-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="397e5-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="397e5-113">initializationVector</span></span>|<span data-ttu-id="397e5-114">Binary</span><span class="sxs-lookup"><span data-stu-id="397e5-114">Binary</span></span>|<span data-ttu-id="397e5-115">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="397e5-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="397e5-116">mac</span><span class="sxs-lookup"><span data-stu-id="397e5-116">mac</span></span>|<span data-ttu-id="397e5-117">Binary</span><span class="sxs-lookup"><span data-stu-id="397e5-117">Binary</span></span>|<span data-ttu-id="397e5-118">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="397e5-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="397e5-119">macKey</span><span class="sxs-lookup"><span data-stu-id="397e5-119">macKey</span></span>|<span data-ttu-id="397e5-120">Binary</span><span class="sxs-lookup"><span data-stu-id="397e5-120">Binary</span></span>|<span data-ttu-id="397e5-121">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="397e5-121">The key used to get mac.</span></span>|
|<span data-ttu-id="397e5-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="397e5-122">profileIdentifier</span></span>|<span data-ttu-id="397e5-123">String</span><span class="sxs-lookup"><span data-stu-id="397e5-123">String</span></span>|<span data-ttu-id="397e5-124">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="397e5-124">The the profile identifier.</span></span>|
|<span data-ttu-id="397e5-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="397e5-125">fileDigest</span></span>|<span data-ttu-id="397e5-126">Binary</span><span class="sxs-lookup"><span data-stu-id="397e5-126">Binary</span></span>|<span data-ttu-id="397e5-127">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="397e5-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="397e5-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="397e5-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="397e5-129">String</span><span class="sxs-lookup"><span data-stu-id="397e5-129">String</span></span>|<span data-ttu-id="397e5-130">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="397e5-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="397e5-131">关系</span><span class="sxs-lookup"><span data-stu-id="397e5-131">Relationships</span></span>
<span data-ttu-id="397e5-132">无</span><span class="sxs-lookup"><span data-stu-id="397e5-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="397e5-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="397e5-133">JSON Representation</span></span>
<span data-ttu-id="397e5-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="397e5-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
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



