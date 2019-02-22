---
title: appLogCollectionDownloadDetails 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3449e1f1a2b8651cea407690019d458d5ac24fa9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147752"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="c298c-103">appLogCollectionDownloadDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="c298c-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="c298c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c298c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c298c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c298c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c298c-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c298c-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c298c-107">属性</span><span class="sxs-lookup"><span data-stu-id="c298c-107">Properties</span></span>
|<span data-ttu-id="c298c-108">属性</span><span class="sxs-lookup"><span data-stu-id="c298c-108">Property</span></span>|<span data-ttu-id="c298c-109">类型</span><span class="sxs-lookup"><span data-stu-id="c298c-109">Type</span></span>|<span data-ttu-id="c298c-110">说明</span><span class="sxs-lookup"><span data-stu-id="c298c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c298c-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="c298c-111">downloadUrl</span></span>|<span data-ttu-id="c298c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="c298c-112">String</span></span>|<span data-ttu-id="c298c-113">下载已完成 AppLogUploadRequest 的 SAS Url</span><span class="sxs-lookup"><span data-stu-id="c298c-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="c298c-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="c298c-114">decryptionKey</span></span>|<span data-ttu-id="c298c-115">字符串</span><span class="sxs-lookup"><span data-stu-id="c298c-115">String</span></span>|<span data-ttu-id="c298c-116">DecryptionKey 作为 string</span><span class="sxs-lookup"><span data-stu-id="c298c-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="c298c-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c298c-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="c298c-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c298c-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="c298c-119">DecryptionAlgorithm 的内容。</span><span class="sxs-lookup"><span data-stu-id="c298c-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="c298c-120">可能的值是`aes256`:。</span><span class="sxs-lookup"><span data-stu-id="c298c-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c298c-121">关系</span><span class="sxs-lookup"><span data-stu-id="c298c-121">Relationships</span></span>
<span data-ttu-id="c298c-122">无</span><span class="sxs-lookup"><span data-stu-id="c298c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c298c-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c298c-123">JSON Representation</span></span>
<span data-ttu-id="c298c-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c298c-124">Here is a JSON representation of the resource.</span></span>
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




