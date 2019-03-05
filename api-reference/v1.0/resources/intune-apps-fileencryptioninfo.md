---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66c4fc3c724eecf3a05dae24cb3f6a52de82d059
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255848"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="8e5cb-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e5cb-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="8e5cb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e5cb-105">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="8e5cb-106">属性</span><span class="sxs-lookup"><span data-stu-id="8e5cb-106">Properties</span></span>
|<span data-ttu-id="8e5cb-107">属性</span><span class="sxs-lookup"><span data-stu-id="8e5cb-107">Property</span></span>|<span data-ttu-id="8e5cb-108">类型</span><span class="sxs-lookup"><span data-stu-id="8e5cb-108">Type</span></span>|<span data-ttu-id="8e5cb-109">说明</span><span class="sxs-lookup"><span data-stu-id="8e5cb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e5cb-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="8e5cb-110">encryptionKey</span></span>|<span data-ttu-id="8e5cb-111">Binary</span><span class="sxs-lookup"><span data-stu-id="8e5cb-111">Binary</span></span>|<span data-ttu-id="8e5cb-112">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="8e5cb-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="8e5cb-113">initializationVector</span></span>|<span data-ttu-id="8e5cb-114">Binary</span><span class="sxs-lookup"><span data-stu-id="8e5cb-114">Binary</span></span>|<span data-ttu-id="8e5cb-115">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="8e5cb-116">mac</span><span class="sxs-lookup"><span data-stu-id="8e5cb-116">mac</span></span>|<span data-ttu-id="8e5cb-117">Binary</span><span class="sxs-lookup"><span data-stu-id="8e5cb-117">Binary</span></span>|<span data-ttu-id="8e5cb-118">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="8e5cb-119">macKey</span><span class="sxs-lookup"><span data-stu-id="8e5cb-119">macKey</span></span>|<span data-ttu-id="8e5cb-120">Binary</span><span class="sxs-lookup"><span data-stu-id="8e5cb-120">Binary</span></span>|<span data-ttu-id="8e5cb-121">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-121">The key used to get mac.</span></span>|
|<span data-ttu-id="8e5cb-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="8e5cb-122">profileIdentifier</span></span>|<span data-ttu-id="8e5cb-123">String</span><span class="sxs-lookup"><span data-stu-id="8e5cb-123">String</span></span>|<span data-ttu-id="8e5cb-124">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-124">The the profile identifier.</span></span>|
|<span data-ttu-id="8e5cb-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="8e5cb-125">fileDigest</span></span>|<span data-ttu-id="8e5cb-126">Binary</span><span class="sxs-lookup"><span data-stu-id="8e5cb-126">Binary</span></span>|<span data-ttu-id="8e5cb-127">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="8e5cb-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8e5cb-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="8e5cb-129">String</span><span class="sxs-lookup"><span data-stu-id="8e5cb-129">String</span></span>|<span data-ttu-id="8e5cb-130">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e5cb-131">关系</span><span class="sxs-lookup"><span data-stu-id="8e5cb-131">Relationships</span></span>
<span data-ttu-id="8e5cb-132">无</span><span class="sxs-lookup"><span data-stu-id="8e5cb-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e5cb-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e5cb-133">JSON Representation</span></span>
<span data-ttu-id="8e5cb-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e5cb-134">Here is a JSON representation of the resource.</span></span>
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



