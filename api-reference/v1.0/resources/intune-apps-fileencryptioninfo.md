---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a6aa144db5b4bc06177af77b965a6268d199105a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029188"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="219a9-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="219a9-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="219a9-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="219a9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="219a9-105">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="219a9-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="219a9-106">属性</span><span class="sxs-lookup"><span data-stu-id="219a9-106">Properties</span></span>
|<span data-ttu-id="219a9-107">属性</span><span class="sxs-lookup"><span data-stu-id="219a9-107">Property</span></span>|<span data-ttu-id="219a9-108">类型</span><span class="sxs-lookup"><span data-stu-id="219a9-108">Type</span></span>|<span data-ttu-id="219a9-109">说明</span><span class="sxs-lookup"><span data-stu-id="219a9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="219a9-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="219a9-110">encryptionKey</span></span>|<span data-ttu-id="219a9-111">Binary</span><span class="sxs-lookup"><span data-stu-id="219a9-111">Binary</span></span>|<span data-ttu-id="219a9-112">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="219a9-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="219a9-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="219a9-113">initializationVector</span></span>|<span data-ttu-id="219a9-114">Binary</span><span class="sxs-lookup"><span data-stu-id="219a9-114">Binary</span></span>|<span data-ttu-id="219a9-115">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="219a9-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="219a9-116">mac</span><span class="sxs-lookup"><span data-stu-id="219a9-116">mac</span></span>|<span data-ttu-id="219a9-117">Binary</span><span class="sxs-lookup"><span data-stu-id="219a9-117">Binary</span></span>|<span data-ttu-id="219a9-118">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="219a9-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="219a9-119">macKey</span><span class="sxs-lookup"><span data-stu-id="219a9-119">macKey</span></span>|<span data-ttu-id="219a9-120">Binary</span><span class="sxs-lookup"><span data-stu-id="219a9-120">Binary</span></span>|<span data-ttu-id="219a9-121">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="219a9-121">The key used to get mac.</span></span>|
|<span data-ttu-id="219a9-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="219a9-122">profileIdentifier</span></span>|<span data-ttu-id="219a9-123">String</span><span class="sxs-lookup"><span data-stu-id="219a9-123">String</span></span>|<span data-ttu-id="219a9-124">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="219a9-124">The profile identifier.</span></span>|
|<span data-ttu-id="219a9-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="219a9-125">fileDigest</span></span>|<span data-ttu-id="219a9-126">Binary</span><span class="sxs-lookup"><span data-stu-id="219a9-126">Binary</span></span>|<span data-ttu-id="219a9-127">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="219a9-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="219a9-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="219a9-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="219a9-129">String</span><span class="sxs-lookup"><span data-stu-id="219a9-129">String</span></span>|<span data-ttu-id="219a9-130">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="219a9-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="219a9-131">关系</span><span class="sxs-lookup"><span data-stu-id="219a9-131">Relationships</span></span>
<span data-ttu-id="219a9-132">无</span><span class="sxs-lookup"><span data-stu-id="219a9-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="219a9-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="219a9-133">JSON Representation</span></span>
<span data-ttu-id="219a9-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="219a9-134">Here is a JSON representation of the resource.</span></span>
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



