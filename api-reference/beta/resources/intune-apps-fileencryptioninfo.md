---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3878f17976f4a3e8fb9b665423b33ebbaa517472
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003924"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="ee0f1-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee0f1-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="ee0f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee0f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee0f1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee0f1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee0f1-107">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="ee0f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee0f1-108">Properties</span></span>
|<span data-ttu-id="ee0f1-109">属性</span><span class="sxs-lookup"><span data-stu-id="ee0f1-109">Property</span></span>|<span data-ttu-id="ee0f1-110">类型</span><span class="sxs-lookup"><span data-stu-id="ee0f1-110">Type</span></span>|<span data-ttu-id="ee0f1-111">说明</span><span class="sxs-lookup"><span data-stu-id="ee0f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee0f1-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="ee0f1-112">encryptionKey</span></span>|<span data-ttu-id="ee0f1-113">Binary</span><span class="sxs-lookup"><span data-stu-id="ee0f1-113">Binary</span></span>|<span data-ttu-id="ee0f1-114">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="ee0f1-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="ee0f1-115">initializationVector</span></span>|<span data-ttu-id="ee0f1-116">Binary</span><span class="sxs-lookup"><span data-stu-id="ee0f1-116">Binary</span></span>|<span data-ttu-id="ee0f1-117">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="ee0f1-118">mac</span><span class="sxs-lookup"><span data-stu-id="ee0f1-118">mac</span></span>|<span data-ttu-id="ee0f1-119">Binary</span><span class="sxs-lookup"><span data-stu-id="ee0f1-119">Binary</span></span>|<span data-ttu-id="ee0f1-120">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="ee0f1-121">macKey</span><span class="sxs-lookup"><span data-stu-id="ee0f1-121">macKey</span></span>|<span data-ttu-id="ee0f1-122">Binary</span><span class="sxs-lookup"><span data-stu-id="ee0f1-122">Binary</span></span>|<span data-ttu-id="ee0f1-123">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-123">The key used to get mac.</span></span>|
|<span data-ttu-id="ee0f1-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="ee0f1-124">profileIdentifier</span></span>|<span data-ttu-id="ee0f1-125">String</span><span class="sxs-lookup"><span data-stu-id="ee0f1-125">String</span></span>|<span data-ttu-id="ee0f1-126">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-126">The the profile identifier.</span></span>|
|<span data-ttu-id="ee0f1-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="ee0f1-127">fileDigest</span></span>|<span data-ttu-id="ee0f1-128">Binary</span><span class="sxs-lookup"><span data-stu-id="ee0f1-128">Binary</span></span>|<span data-ttu-id="ee0f1-129">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="ee0f1-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ee0f1-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="ee0f1-131">String</span><span class="sxs-lookup"><span data-stu-id="ee0f1-131">String</span></span>|<span data-ttu-id="ee0f1-132">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee0f1-133">关系</span><span class="sxs-lookup"><span data-stu-id="ee0f1-133">Relationships</span></span>
<span data-ttu-id="ee0f1-134">无</span><span class="sxs-lookup"><span data-stu-id="ee0f1-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee0f1-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee0f1-135">JSON Representation</span></span>
<span data-ttu-id="ee0f1-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee0f1-136">Here is a JSON representation of the resource.</span></span>
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






