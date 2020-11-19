---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5bb90354172fab1f691a49b2488871109df3532
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274269"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="cd7e8-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd7e8-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="cd7e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd7e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd7e8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd7e8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd7e8-107">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="cd7e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd7e8-108">Properties</span></span>
|<span data-ttu-id="cd7e8-109">属性</span><span class="sxs-lookup"><span data-stu-id="cd7e8-109">Property</span></span>|<span data-ttu-id="cd7e8-110">类型</span><span class="sxs-lookup"><span data-stu-id="cd7e8-110">Type</span></span>|<span data-ttu-id="cd7e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="cd7e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd7e8-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="cd7e8-112">encryptionKey</span></span>|<span data-ttu-id="cd7e8-113">Binary</span><span class="sxs-lookup"><span data-stu-id="cd7e8-113">Binary</span></span>|<span data-ttu-id="cd7e8-114">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="cd7e8-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="cd7e8-115">initializationVector</span></span>|<span data-ttu-id="cd7e8-116">Binary</span><span class="sxs-lookup"><span data-stu-id="cd7e8-116">Binary</span></span>|<span data-ttu-id="cd7e8-117">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="cd7e8-118">mac</span><span class="sxs-lookup"><span data-stu-id="cd7e8-118">mac</span></span>|<span data-ttu-id="cd7e8-119">Binary</span><span class="sxs-lookup"><span data-stu-id="cd7e8-119">Binary</span></span>|<span data-ttu-id="cd7e8-120">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="cd7e8-121">macKey</span><span class="sxs-lookup"><span data-stu-id="cd7e8-121">macKey</span></span>|<span data-ttu-id="cd7e8-122">Binary</span><span class="sxs-lookup"><span data-stu-id="cd7e8-122">Binary</span></span>|<span data-ttu-id="cd7e8-123">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-123">The key used to get mac.</span></span>|
|<span data-ttu-id="cd7e8-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="cd7e8-124">profileIdentifier</span></span>|<span data-ttu-id="cd7e8-125">String</span><span class="sxs-lookup"><span data-stu-id="cd7e8-125">String</span></span>|<span data-ttu-id="cd7e8-126">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-126">The the profile identifier.</span></span>|
|<span data-ttu-id="cd7e8-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="cd7e8-127">fileDigest</span></span>|<span data-ttu-id="cd7e8-128">Binary</span><span class="sxs-lookup"><span data-stu-id="cd7e8-128">Binary</span></span>|<span data-ttu-id="cd7e8-129">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="cd7e8-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="cd7e8-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="cd7e8-131">String</span><span class="sxs-lookup"><span data-stu-id="cd7e8-131">String</span></span>|<span data-ttu-id="cd7e8-132">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd7e8-133">关系</span><span class="sxs-lookup"><span data-stu-id="cd7e8-133">Relationships</span></span>
<span data-ttu-id="cd7e8-134">无</span><span class="sxs-lookup"><span data-stu-id="cd7e8-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd7e8-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd7e8-135">JSON Representation</span></span>
<span data-ttu-id="cd7e8-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd7e8-136">Here is a JSON representation of the resource.</span></span>
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




