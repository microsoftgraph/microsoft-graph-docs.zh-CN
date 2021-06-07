---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f22c1d25b45b31cf682ad95d573fe3b41534dc9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755607"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="0ae3c-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ae3c-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="0ae3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ae3c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ae3c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ae3c-106">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="0ae3c-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ae3c-107">Properties</span></span>
|<span data-ttu-id="0ae3c-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ae3c-108">Property</span></span>|<span data-ttu-id="0ae3c-109">类型</span><span class="sxs-lookup"><span data-stu-id="0ae3c-109">Type</span></span>|<span data-ttu-id="0ae3c-110">说明</span><span class="sxs-lookup"><span data-stu-id="0ae3c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ae3c-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="0ae3c-111">encryptionKey</span></span>|<span data-ttu-id="0ae3c-112">Binary</span><span class="sxs-lookup"><span data-stu-id="0ae3c-112">Binary</span></span>|<span data-ttu-id="0ae3c-113">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="0ae3c-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="0ae3c-114">initializationVector</span></span>|<span data-ttu-id="0ae3c-115">Binary</span><span class="sxs-lookup"><span data-stu-id="0ae3c-115">Binary</span></span>|<span data-ttu-id="0ae3c-116">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="0ae3c-117">mac</span><span class="sxs-lookup"><span data-stu-id="0ae3c-117">mac</span></span>|<span data-ttu-id="0ae3c-118">Binary</span><span class="sxs-lookup"><span data-stu-id="0ae3c-118">Binary</span></span>|<span data-ttu-id="0ae3c-119">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="0ae3c-120">macKey</span><span class="sxs-lookup"><span data-stu-id="0ae3c-120">macKey</span></span>|<span data-ttu-id="0ae3c-121">Binary</span><span class="sxs-lookup"><span data-stu-id="0ae3c-121">Binary</span></span>|<span data-ttu-id="0ae3c-122">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-122">The key used to get mac.</span></span>|
|<span data-ttu-id="0ae3c-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="0ae3c-123">profileIdentifier</span></span>|<span data-ttu-id="0ae3c-124">String</span><span class="sxs-lookup"><span data-stu-id="0ae3c-124">String</span></span>|<span data-ttu-id="0ae3c-125">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-125">The the profile identifier.</span></span>|
|<span data-ttu-id="0ae3c-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="0ae3c-126">fileDigest</span></span>|<span data-ttu-id="0ae3c-127">Binary</span><span class="sxs-lookup"><span data-stu-id="0ae3c-127">Binary</span></span>|<span data-ttu-id="0ae3c-128">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="0ae3c-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="0ae3c-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="0ae3c-130">String</span><span class="sxs-lookup"><span data-stu-id="0ae3c-130">String</span></span>|<span data-ttu-id="0ae3c-131">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ae3c-132">关系</span><span class="sxs-lookup"><span data-stu-id="0ae3c-132">Relationships</span></span>
<span data-ttu-id="0ae3c-133">无</span><span class="sxs-lookup"><span data-stu-id="0ae3c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ae3c-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ae3c-134">JSON Representation</span></span>
<span data-ttu-id="0ae3c-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ae3c-135">Here is a JSON representation of the resource.</span></span>
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




