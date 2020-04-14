---
title: appLogCollectionDownloadDetails 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dade0c3a266e8cba801a8e88dacebda6bbd2d197
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465254"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="69a32-103">appLogCollectionDownloadDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="69a32-103">appLogCollectionDownloadDetails resource type</span></span>

<span data-ttu-id="69a32-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69a32-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69a32-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69a32-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69a32-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69a32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69a32-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69a32-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="69a32-108">属性</span><span class="sxs-lookup"><span data-stu-id="69a32-108">Properties</span></span>
|<span data-ttu-id="69a32-109">属性</span><span class="sxs-lookup"><span data-stu-id="69a32-109">Property</span></span>|<span data-ttu-id="69a32-110">类型</span><span class="sxs-lookup"><span data-stu-id="69a32-110">Type</span></span>|<span data-ttu-id="69a32-111">说明</span><span class="sxs-lookup"><span data-stu-id="69a32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69a32-112">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="69a32-112">downloadUrl</span></span>|<span data-ttu-id="69a32-113">String</span><span class="sxs-lookup"><span data-stu-id="69a32-113">String</span></span>|<span data-ttu-id="69a32-114">下载已完成 AppLogUploadRequest 的 SAS Url</span><span class="sxs-lookup"><span data-stu-id="69a32-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="69a32-115">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="69a32-115">decryptionKey</span></span>|<span data-ttu-id="69a32-116">String</span><span class="sxs-lookup"><span data-stu-id="69a32-116">String</span></span>|<span data-ttu-id="69a32-117">DecryptionKey 作为 string</span><span class="sxs-lookup"><span data-stu-id="69a32-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="69a32-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="69a32-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="69a32-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="69a32-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="69a32-120">DecryptionAlgorithm 的内容。</span><span class="sxs-lookup"><span data-stu-id="69a32-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="69a32-121">可能的值是`aes256`：。</span><span class="sxs-lookup"><span data-stu-id="69a32-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69a32-122">关系</span><span class="sxs-lookup"><span data-stu-id="69a32-122">Relationships</span></span>
<span data-ttu-id="69a32-123">无</span><span class="sxs-lookup"><span data-stu-id="69a32-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69a32-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69a32-124">JSON Representation</span></span>
<span data-ttu-id="69a32-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69a32-125">Here is a JSON representation of the resource.</span></span>
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



