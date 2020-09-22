---
title: appLogCollectionDownloadDetails 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53931e6a07f5d531e0661d4f56a720a9b6b560bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060879"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="2b1b3-103">appLogCollectionDownloadDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b1b3-103">appLogCollectionDownloadDetails resource type</span></span>

<span data-ttu-id="2b1b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b1b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b1b3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b1b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b1b3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b1b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b1b3-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2b1b3-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2b1b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b1b3-108">Properties</span></span>
|<span data-ttu-id="2b1b3-109">属性</span><span class="sxs-lookup"><span data-stu-id="2b1b3-109">Property</span></span>|<span data-ttu-id="2b1b3-110">类型</span><span class="sxs-lookup"><span data-stu-id="2b1b3-110">Type</span></span>|<span data-ttu-id="2b1b3-111">说明</span><span class="sxs-lookup"><span data-stu-id="2b1b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b1b3-112">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="2b1b3-112">downloadUrl</span></span>|<span data-ttu-id="2b1b3-113">String</span><span class="sxs-lookup"><span data-stu-id="2b1b3-113">String</span></span>|<span data-ttu-id="2b1b3-114">下载已完成 AppLogUploadRequest 的 SAS Url</span><span class="sxs-lookup"><span data-stu-id="2b1b3-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="2b1b3-115">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="2b1b3-115">decryptionKey</span></span>|<span data-ttu-id="2b1b3-116">String</span><span class="sxs-lookup"><span data-stu-id="2b1b3-116">String</span></span>|<span data-ttu-id="2b1b3-117">DecryptionKey 作为 string</span><span class="sxs-lookup"><span data-stu-id="2b1b3-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="2b1b3-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="2b1b3-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="2b1b3-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="2b1b3-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="2b1b3-120">DecryptionAlgorithm 的内容。</span><span class="sxs-lookup"><span data-stu-id="2b1b3-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="2b1b3-121">可能的值是： `aes256` 。</span><span class="sxs-lookup"><span data-stu-id="2b1b3-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b1b3-122">关系</span><span class="sxs-lookup"><span data-stu-id="2b1b3-122">Relationships</span></span>
<span data-ttu-id="2b1b3-123">无</span><span class="sxs-lookup"><span data-stu-id="2b1b3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b1b3-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b1b3-124">JSON Representation</span></span>
<span data-ttu-id="2b1b3-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b1b3-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```






