---
title: appLogCollectionDownloadDetails 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c581b6ffe1653c2962c03c8e6fe5d27d706882d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549416"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="6d7e6-103">appLogCollectionDownloadDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d7e6-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="6d7e6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d7e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d7e6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d7e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d7e6-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d7e6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6d7e6-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d7e6-107">Properties</span></span>
|<span data-ttu-id="6d7e6-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d7e6-108">Property</span></span>|<span data-ttu-id="6d7e6-109">类型</span><span class="sxs-lookup"><span data-stu-id="6d7e6-109">Type</span></span>|<span data-ttu-id="6d7e6-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d7e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d7e6-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="6d7e6-111">downloadUrl</span></span>|<span data-ttu-id="6d7e6-112">String</span><span class="sxs-lookup"><span data-stu-id="6d7e6-112">String</span></span>|<span data-ttu-id="6d7e6-113">下载已完成 AppLogUploadRequest 的 SAS Url</span><span class="sxs-lookup"><span data-stu-id="6d7e6-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="6d7e6-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="6d7e6-114">decryptionKey</span></span>|<span data-ttu-id="6d7e6-115">String</span><span class="sxs-lookup"><span data-stu-id="6d7e6-115">String</span></span>|<span data-ttu-id="6d7e6-116">DecryptionKey 作为 string</span><span class="sxs-lookup"><span data-stu-id="6d7e6-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="6d7e6-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="6d7e6-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="6d7e6-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="6d7e6-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="6d7e6-119">DecryptionAlgorithm 的内容。</span><span class="sxs-lookup"><span data-stu-id="6d7e6-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="6d7e6-120">可能的值是`aes256`:。</span><span class="sxs-lookup"><span data-stu-id="6d7e6-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d7e6-121">关系</span><span class="sxs-lookup"><span data-stu-id="6d7e6-121">Relationships</span></span>
<span data-ttu-id="6d7e6-122">无</span><span class="sxs-lookup"><span data-stu-id="6d7e6-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d7e6-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d7e6-123">JSON Representation</span></span>
<span data-ttu-id="6d7e6-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d7e6-124">Here is a JSON representation of the resource.</span></span>
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





