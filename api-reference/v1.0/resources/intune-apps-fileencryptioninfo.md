---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e0dff917b9fc6dc8bc99cb388cdf0f461dc394c3
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356287"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="c7107-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7107-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="c7107-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7107-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7107-105">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="c7107-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="c7107-106">属性</span><span class="sxs-lookup"><span data-stu-id="c7107-106">Properties</span></span>
|<span data-ttu-id="c7107-107">属性</span><span class="sxs-lookup"><span data-stu-id="c7107-107">Property</span></span>|<span data-ttu-id="c7107-108">类型</span><span class="sxs-lookup"><span data-stu-id="c7107-108">Type</span></span>|<span data-ttu-id="c7107-109">说明</span><span class="sxs-lookup"><span data-stu-id="c7107-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7107-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="c7107-110">encryptionKey</span></span>|<span data-ttu-id="c7107-111">Binary</span><span class="sxs-lookup"><span data-stu-id="c7107-111">Binary</span></span>|<span data-ttu-id="c7107-112">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="c7107-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="c7107-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="c7107-113">initializationVector</span></span>|<span data-ttu-id="c7107-114">Binary</span><span class="sxs-lookup"><span data-stu-id="c7107-114">Binary</span></span>|<span data-ttu-id="c7107-115">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="c7107-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="c7107-116">mac</span><span class="sxs-lookup"><span data-stu-id="c7107-116">mac</span></span>|<span data-ttu-id="c7107-117">Binary</span><span class="sxs-lookup"><span data-stu-id="c7107-117">Binary</span></span>|<span data-ttu-id="c7107-118">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="c7107-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="c7107-119">macKey</span><span class="sxs-lookup"><span data-stu-id="c7107-119">macKey</span></span>|<span data-ttu-id="c7107-120">Binary</span><span class="sxs-lookup"><span data-stu-id="c7107-120">Binary</span></span>|<span data-ttu-id="c7107-121">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="c7107-121">The key used to get mac.</span></span>|
|<span data-ttu-id="c7107-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="c7107-122">profileIdentifier</span></span>|<span data-ttu-id="c7107-123">String</span><span class="sxs-lookup"><span data-stu-id="c7107-123">String</span></span>|<span data-ttu-id="c7107-124">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="c7107-124">The profile identifier.</span></span>|
|<span data-ttu-id="c7107-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="c7107-125">fileDigest</span></span>|<span data-ttu-id="c7107-126">Binary</span><span class="sxs-lookup"><span data-stu-id="c7107-126">Binary</span></span>|<span data-ttu-id="c7107-127">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="c7107-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="c7107-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c7107-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="c7107-129">String</span><span class="sxs-lookup"><span data-stu-id="c7107-129">String</span></span>|<span data-ttu-id="c7107-130">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="c7107-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7107-131">关系</span><span class="sxs-lookup"><span data-stu-id="c7107-131">Relationships</span></span>
<span data-ttu-id="c7107-132">无</span><span class="sxs-lookup"><span data-stu-id="c7107-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7107-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7107-133">JSON Representation</span></span>
<span data-ttu-id="c7107-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7107-134">Here is a JSON representation of the resource.</span></span>
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




