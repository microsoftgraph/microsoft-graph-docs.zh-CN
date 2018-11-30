---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
ms.openlocfilehash: 17895b0bf081cc249f9081c737a2445683514280
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042523"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="ba30a-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba30a-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="ba30a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ba30a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba30a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ba30a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba30a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ba30a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba30a-107">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="ba30a-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="ba30a-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba30a-108">Properties</span></span>
|<span data-ttu-id="ba30a-109">属性</span><span class="sxs-lookup"><span data-stu-id="ba30a-109">Property</span></span>|<span data-ttu-id="ba30a-110">类型</span><span class="sxs-lookup"><span data-stu-id="ba30a-110">Type</span></span>|<span data-ttu-id="ba30a-111">说明</span><span class="sxs-lookup"><span data-stu-id="ba30a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba30a-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="ba30a-112">encryptionKey</span></span>|<span data-ttu-id="ba30a-113">Binary</span><span class="sxs-lookup"><span data-stu-id="ba30a-113">Binary</span></span>|<span data-ttu-id="ba30a-114">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="ba30a-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="ba30a-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="ba30a-115">initializationVector</span></span>|<span data-ttu-id="ba30a-116">Binary</span><span class="sxs-lookup"><span data-stu-id="ba30a-116">Binary</span></span>|<span data-ttu-id="ba30a-117">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="ba30a-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="ba30a-118">mac</span><span class="sxs-lookup"><span data-stu-id="ba30a-118">mac</span></span>|<span data-ttu-id="ba30a-119">Binary</span><span class="sxs-lookup"><span data-stu-id="ba30a-119">Binary</span></span>|<span data-ttu-id="ba30a-120">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="ba30a-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="ba30a-121">macKey</span><span class="sxs-lookup"><span data-stu-id="ba30a-121">macKey</span></span>|<span data-ttu-id="ba30a-122">Binary</span><span class="sxs-lookup"><span data-stu-id="ba30a-122">Binary</span></span>|<span data-ttu-id="ba30a-123">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="ba30a-123">The key used to get mac.</span></span>|
|<span data-ttu-id="ba30a-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="ba30a-124">profileIdentifier</span></span>|<span data-ttu-id="ba30a-125">String</span><span class="sxs-lookup"><span data-stu-id="ba30a-125">String</span></span>|<span data-ttu-id="ba30a-126">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="ba30a-126">The the profile identifier.</span></span>|
|<span data-ttu-id="ba30a-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="ba30a-127">fileDigest</span></span>|<span data-ttu-id="ba30a-128">Binary</span><span class="sxs-lookup"><span data-stu-id="ba30a-128">Binary</span></span>|<span data-ttu-id="ba30a-129">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="ba30a-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="ba30a-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ba30a-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="ba30a-131">String</span><span class="sxs-lookup"><span data-stu-id="ba30a-131">String</span></span>|<span data-ttu-id="ba30a-132">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="ba30a-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba30a-133">关系</span><span class="sxs-lookup"><span data-stu-id="ba30a-133">Relationships</span></span>
<span data-ttu-id="ba30a-134">无</span><span class="sxs-lookup"><span data-stu-id="ba30a-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ba30a-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba30a-135">JSON Representation</span></span>
<span data-ttu-id="ba30a-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba30a-136">Here is a JSON representation of the resource.</span></span>
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





