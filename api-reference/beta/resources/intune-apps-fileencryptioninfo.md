---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5717936692dde3e92071e0f697fa0204bf7550ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493788"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="e883d-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="e883d-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="e883d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e883d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e883d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e883d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e883d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e883d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e883d-107">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="e883d-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="e883d-108">属性</span><span class="sxs-lookup"><span data-stu-id="e883d-108">Properties</span></span>
|<span data-ttu-id="e883d-109">属性</span><span class="sxs-lookup"><span data-stu-id="e883d-109">Property</span></span>|<span data-ttu-id="e883d-110">类型</span><span class="sxs-lookup"><span data-stu-id="e883d-110">Type</span></span>|<span data-ttu-id="e883d-111">说明</span><span class="sxs-lookup"><span data-stu-id="e883d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e883d-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="e883d-112">encryptionKey</span></span>|<span data-ttu-id="e883d-113">Binary</span><span class="sxs-lookup"><span data-stu-id="e883d-113">Binary</span></span>|<span data-ttu-id="e883d-114">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="e883d-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="e883d-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="e883d-115">initializationVector</span></span>|<span data-ttu-id="e883d-116">Binary</span><span class="sxs-lookup"><span data-stu-id="e883d-116">Binary</span></span>|<span data-ttu-id="e883d-117">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="e883d-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="e883d-118">mac</span><span class="sxs-lookup"><span data-stu-id="e883d-118">mac</span></span>|<span data-ttu-id="e883d-119">Binary</span><span class="sxs-lookup"><span data-stu-id="e883d-119">Binary</span></span>|<span data-ttu-id="e883d-120">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="e883d-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="e883d-121">macKey</span><span class="sxs-lookup"><span data-stu-id="e883d-121">macKey</span></span>|<span data-ttu-id="e883d-122">Binary</span><span class="sxs-lookup"><span data-stu-id="e883d-122">Binary</span></span>|<span data-ttu-id="e883d-123">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="e883d-123">The key used to get mac.</span></span>|
|<span data-ttu-id="e883d-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="e883d-124">profileIdentifier</span></span>|<span data-ttu-id="e883d-125">String</span><span class="sxs-lookup"><span data-stu-id="e883d-125">String</span></span>|<span data-ttu-id="e883d-126">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="e883d-126">The the profile identifier.</span></span>|
|<span data-ttu-id="e883d-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="e883d-127">fileDigest</span></span>|<span data-ttu-id="e883d-128">Binary</span><span class="sxs-lookup"><span data-stu-id="e883d-128">Binary</span></span>|<span data-ttu-id="e883d-129">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="e883d-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="e883d-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e883d-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="e883d-131">String</span><span class="sxs-lookup"><span data-stu-id="e883d-131">String</span></span>|<span data-ttu-id="e883d-132">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="e883d-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e883d-133">关系</span><span class="sxs-lookup"><span data-stu-id="e883d-133">Relationships</span></span>
<span data-ttu-id="e883d-134">无</span><span class="sxs-lookup"><span data-stu-id="e883d-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e883d-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e883d-135">JSON Representation</span></span>
<span data-ttu-id="e883d-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e883d-136">Here is a JSON representation of the resource.</span></span>
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



