---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ed56f695da8dece64702472cd3822603e02dd8b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840689"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="e0d15-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0d15-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="e0d15-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e0d15-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0d15-105">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="e0d15-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="e0d15-106">属性</span><span class="sxs-lookup"><span data-stu-id="e0d15-106">Properties</span></span>
|<span data-ttu-id="e0d15-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0d15-107">Property</span></span>|<span data-ttu-id="e0d15-108">类型</span><span class="sxs-lookup"><span data-stu-id="e0d15-108">Type</span></span>|<span data-ttu-id="e0d15-109">说明</span><span class="sxs-lookup"><span data-stu-id="e0d15-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0d15-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="e0d15-110">encryptionKey</span></span>|<span data-ttu-id="e0d15-111">Binary</span><span class="sxs-lookup"><span data-stu-id="e0d15-111">Binary</span></span>|<span data-ttu-id="e0d15-112">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="e0d15-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="e0d15-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="e0d15-113">initializationVector</span></span>|<span data-ttu-id="e0d15-114">Binary</span><span class="sxs-lookup"><span data-stu-id="e0d15-114">Binary</span></span>|<span data-ttu-id="e0d15-115">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="e0d15-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="e0d15-116">mac</span><span class="sxs-lookup"><span data-stu-id="e0d15-116">mac</span></span>|<span data-ttu-id="e0d15-117">Binary</span><span class="sxs-lookup"><span data-stu-id="e0d15-117">Binary</span></span>|<span data-ttu-id="e0d15-118">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="e0d15-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="e0d15-119">macKey</span><span class="sxs-lookup"><span data-stu-id="e0d15-119">macKey</span></span>|<span data-ttu-id="e0d15-120">Binary</span><span class="sxs-lookup"><span data-stu-id="e0d15-120">Binary</span></span>|<span data-ttu-id="e0d15-121">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="e0d15-121">The key used to get mac.</span></span>|
|<span data-ttu-id="e0d15-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="e0d15-122">profileIdentifier</span></span>|<span data-ttu-id="e0d15-123">String</span><span class="sxs-lookup"><span data-stu-id="e0d15-123">String</span></span>|<span data-ttu-id="e0d15-124">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="e0d15-124">The the profile identifier.</span></span>|
|<span data-ttu-id="e0d15-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="e0d15-125">fileDigest</span></span>|<span data-ttu-id="e0d15-126">Binary</span><span class="sxs-lookup"><span data-stu-id="e0d15-126">Binary</span></span>|<span data-ttu-id="e0d15-127">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="e0d15-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="e0d15-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e0d15-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="e0d15-129">String</span><span class="sxs-lookup"><span data-stu-id="e0d15-129">String</span></span>|<span data-ttu-id="e0d15-130">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="e0d15-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0d15-131">关系</span><span class="sxs-lookup"><span data-stu-id="e0d15-131">Relationships</span></span>
<span data-ttu-id="e0d15-132">无</span><span class="sxs-lookup"><span data-stu-id="e0d15-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0d15-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0d15-133">JSON Representation</span></span>
<span data-ttu-id="e0d15-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0d15-134">Here is a JSON representation of the resource.</span></span>
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



