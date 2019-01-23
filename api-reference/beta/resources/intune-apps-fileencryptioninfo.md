---
title: fileEncryptionInfo 资源类型
description: 包含业务线应用内容版本文件加密信息的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 074bf24638bf0ba7d613399e1b8894de7f30dfbb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410894"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="5b4da-103">fileEncryptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b4da-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="5b4da-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5b4da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5b4da-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b4da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b4da-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b4da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b4da-107">包含业务线应用内容版本文件加密信息的属性。</span><span class="sxs-lookup"><span data-stu-id="5b4da-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="5b4da-108">属性</span><span class="sxs-lookup"><span data-stu-id="5b4da-108">Properties</span></span>
|<span data-ttu-id="5b4da-109">属性</span><span class="sxs-lookup"><span data-stu-id="5b4da-109">Property</span></span>|<span data-ttu-id="5b4da-110">类型</span><span class="sxs-lookup"><span data-stu-id="5b4da-110">Type</span></span>|<span data-ttu-id="5b4da-111">说明</span><span class="sxs-lookup"><span data-stu-id="5b4da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b4da-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="5b4da-112">encryptionKey</span></span>|<span data-ttu-id="5b4da-113">Binary</span><span class="sxs-lookup"><span data-stu-id="5b4da-113">Binary</span></span>|<span data-ttu-id="5b4da-114">用于加密文件内容的密钥。</span><span class="sxs-lookup"><span data-stu-id="5b4da-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="5b4da-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="5b4da-115">initializationVector</span></span>|<span data-ttu-id="5b4da-116">Binary</span><span class="sxs-lookup"><span data-stu-id="5b4da-116">Binary</span></span>|<span data-ttu-id="5b4da-117">用于加密算法的初始化向量。</span><span class="sxs-lookup"><span data-stu-id="5b4da-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="5b4da-118">mac</span><span class="sxs-lookup"><span data-stu-id="5b4da-118">mac</span></span>|<span data-ttu-id="5b4da-119">Binary</span><span class="sxs-lookup"><span data-stu-id="5b4da-119">Binary</span></span>|<span data-ttu-id="5b4da-120">加密文件内容和 IV 的哈希（内容哈希）。</span><span class="sxs-lookup"><span data-stu-id="5b4da-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="5b4da-121">macKey</span><span class="sxs-lookup"><span data-stu-id="5b4da-121">macKey</span></span>|<span data-ttu-id="5b4da-122">Binary</span><span class="sxs-lookup"><span data-stu-id="5b4da-122">Binary</span></span>|<span data-ttu-id="5b4da-123">用于获取 mac 的密钥。</span><span class="sxs-lookup"><span data-stu-id="5b4da-123">The key used to get mac.</span></span>|
|<span data-ttu-id="5b4da-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="5b4da-124">profileIdentifier</span></span>|<span data-ttu-id="5b4da-125">String</span><span class="sxs-lookup"><span data-stu-id="5b4da-125">String</span></span>|<span data-ttu-id="5b4da-126">配置文件标识符。</span><span class="sxs-lookup"><span data-stu-id="5b4da-126">The the profile identifier.</span></span>|
|<span data-ttu-id="5b4da-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="5b4da-127">fileDigest</span></span>|<span data-ttu-id="5b4da-128">Binary</span><span class="sxs-lookup"><span data-stu-id="5b4da-128">Binary</span></span>|<span data-ttu-id="5b4da-129">加密前的文件摘要。</span><span class="sxs-lookup"><span data-stu-id="5b4da-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="5b4da-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="5b4da-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="5b4da-131">String</span><span class="sxs-lookup"><span data-stu-id="5b4da-131">String</span></span>|<span data-ttu-id="5b4da-132">文件摘要算法。</span><span class="sxs-lookup"><span data-stu-id="5b4da-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b4da-133">关系</span><span class="sxs-lookup"><span data-stu-id="5b4da-133">Relationships</span></span>
<span data-ttu-id="5b4da-134">无</span><span class="sxs-lookup"><span data-stu-id="5b4da-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b4da-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b4da-135">JSON Representation</span></span>
<span data-ttu-id="5b4da-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b4da-136">Here is a JSON representation of the resource.</span></span>
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




