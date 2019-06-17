---
title: appLogCollectionDownloadDetails 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2347bbe60b3bf7bab0cbdc6dcffb35b8489a3e14
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983328"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="95044-103">appLogCollectionDownloadDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="95044-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="95044-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95044-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95044-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95044-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95044-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="95044-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="95044-107">属性</span><span class="sxs-lookup"><span data-stu-id="95044-107">Properties</span></span>
|<span data-ttu-id="95044-108">属性</span><span class="sxs-lookup"><span data-stu-id="95044-108">Property</span></span>|<span data-ttu-id="95044-109">类型</span><span class="sxs-lookup"><span data-stu-id="95044-109">Type</span></span>|<span data-ttu-id="95044-110">说明</span><span class="sxs-lookup"><span data-stu-id="95044-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95044-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="95044-111">downloadUrl</span></span>|<span data-ttu-id="95044-112">String</span><span class="sxs-lookup"><span data-stu-id="95044-112">String</span></span>|<span data-ttu-id="95044-113">下载已完成 AppLogUploadRequest 的 SAS Url</span><span class="sxs-lookup"><span data-stu-id="95044-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="95044-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="95044-114">decryptionKey</span></span>|<span data-ttu-id="95044-115">String</span><span class="sxs-lookup"><span data-stu-id="95044-115">String</span></span>|<span data-ttu-id="95044-116">DecryptionKey 作为 string</span><span class="sxs-lookup"><span data-stu-id="95044-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="95044-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="95044-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="95044-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="95044-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="95044-119">DecryptionAlgorithm 的内容。</span><span class="sxs-lookup"><span data-stu-id="95044-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="95044-120">可能的值是`aes256`:。</span><span class="sxs-lookup"><span data-stu-id="95044-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95044-121">关系</span><span class="sxs-lookup"><span data-stu-id="95044-121">Relationships</span></span>
<span data-ttu-id="95044-122">无</span><span class="sxs-lookup"><span data-stu-id="95044-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95044-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95044-123">JSON Representation</span></span>
<span data-ttu-id="95044-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95044-124">Here is a JSON representation of the resource.</span></span>
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





