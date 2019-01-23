---
title: appLogCollectionDownloadDetails 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6946b3cd1aa60c4025859bd8d41d2dc4775bf39d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429272"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="d289f-103">appLogCollectionDownloadDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="d289f-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="d289f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d289f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d289f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d289f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d289f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d289f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d289f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d289f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d289f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d289f-108">Properties</span></span>
|<span data-ttu-id="d289f-109">属性</span><span class="sxs-lookup"><span data-stu-id="d289f-109">Property</span></span>|<span data-ttu-id="d289f-110">类型</span><span class="sxs-lookup"><span data-stu-id="d289f-110">Type</span></span>|<span data-ttu-id="d289f-111">说明</span><span class="sxs-lookup"><span data-stu-id="d289f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d289f-112">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="d289f-112">downloadUrl</span></span>|<span data-ttu-id="d289f-113">String</span><span class="sxs-lookup"><span data-stu-id="d289f-113">String</span></span>|<span data-ttu-id="d289f-114">已完成 AppLogUploadRequest 下载 SAS Url</span><span class="sxs-lookup"><span data-stu-id="d289f-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="d289f-115">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="d289f-115">decryptionKey</span></span>|<span data-ttu-id="d289f-116">String</span><span class="sxs-lookup"><span data-stu-id="d289f-116">String</span></span>|<span data-ttu-id="d289f-117">作为字符串 DecryptionKey</span><span class="sxs-lookup"><span data-stu-id="d289f-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="d289f-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d289f-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="d289f-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d289f-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="d289f-120">内容 DecryptionAlgorithm。</span><span class="sxs-lookup"><span data-stu-id="d289f-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="d289f-121">可能的值为： `aes256`。</span><span class="sxs-lookup"><span data-stu-id="d289f-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d289f-122">关系</span><span class="sxs-lookup"><span data-stu-id="d289f-122">Relationships</span></span>
<span data-ttu-id="d289f-123">无</span><span class="sxs-lookup"><span data-stu-id="d289f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d289f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d289f-124">JSON Representation</span></span>
<span data-ttu-id="d289f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d289f-125">Here is a JSON representation of the resource.</span></span>
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




