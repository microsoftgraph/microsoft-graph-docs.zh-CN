---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 528c68b352f45a4b029a09c37585eda2be540d1a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620197"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="edd43-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="edd43-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="edd43-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="edd43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edd43-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="edd43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edd43-106">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="edd43-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="edd43-107">属性</span><span class="sxs-lookup"><span data-stu-id="edd43-107">Properties</span></span>
|<span data-ttu-id="edd43-108">属性</span><span class="sxs-lookup"><span data-stu-id="edd43-108">Property</span></span>|<span data-ttu-id="edd43-109">类型</span><span class="sxs-lookup"><span data-stu-id="edd43-109">Type</span></span>|<span data-ttu-id="edd43-110">说明</span><span class="sxs-lookup"><span data-stu-id="edd43-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edd43-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="edd43-111">encryptionKey</span></span>|<span data-ttu-id="edd43-112">Binary</span><span class="sxs-lookup"><span data-stu-id="edd43-112">Binary</span></span>|<span data-ttu-id="edd43-113">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="edd43-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="edd43-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="edd43-114">initializationVector</span></span>|<span data-ttu-id="edd43-115">Binary</span><span class="sxs-lookup"><span data-stu-id="edd43-115">Binary</span></span>|<span data-ttu-id="edd43-116">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="edd43-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="edd43-117">mac</span><span class="sxs-lookup"><span data-stu-id="edd43-117">mac</span></span>|<span data-ttu-id="edd43-118">Binary</span><span class="sxs-lookup"><span data-stu-id="edd43-118">Binary</span></span>|<span data-ttu-id="edd43-119">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="edd43-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="edd43-120">macKey</span><span class="sxs-lookup"><span data-stu-id="edd43-120">macKey</span></span>|<span data-ttu-id="edd43-121">Binary</span><span class="sxs-lookup"><span data-stu-id="edd43-121">Binary</span></span>|<span data-ttu-id="edd43-122">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="edd43-122">The key used to get mac.</span></span>|
|<span data-ttu-id="edd43-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="edd43-123">profileIdentifier</span></span>|<span data-ttu-id="edd43-124">String</span><span class="sxs-lookup"><span data-stu-id="edd43-124">String</span></span>|<span data-ttu-id="edd43-125">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="edd43-125">The profile identifier.</span></span>|
|<span data-ttu-id="edd43-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="edd43-126">fileDigest</span></span>|<span data-ttu-id="edd43-127">Binary</span><span class="sxs-lookup"><span data-stu-id="edd43-127">Binary</span></span>|<span data-ttu-id="edd43-128">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="edd43-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="edd43-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="edd43-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="edd43-130">String</span><span class="sxs-lookup"><span data-stu-id="edd43-130">String</span></span>|<span data-ttu-id="edd43-131">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="edd43-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edd43-132">关系</span><span class="sxs-lookup"><span data-stu-id="edd43-132">Relationships</span></span>
<span data-ttu-id="edd43-133">无</span><span class="sxs-lookup"><span data-stu-id="edd43-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="edd43-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edd43-134">JSON Representation</span></span>
<span data-ttu-id="edd43-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edd43-135">Here is a JSON representation of the resource.</span></span>
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





