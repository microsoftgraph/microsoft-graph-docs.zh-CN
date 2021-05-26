---
title: officeUserCheckinSummary 资源类型
description: 描述租户签入统计数据的实体。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed81c3c152b0d81cfcdf15388fdc4db3a7612052
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666861"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="926b7-103">officeUserCheckinSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="926b7-103">officeUserCheckinSummary resource type</span></span>

<span data-ttu-id="926b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="926b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="926b7-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="926b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="926b7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="926b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="926b7-107">描述租户签入统计数据的实体。</span><span class="sxs-lookup"><span data-stu-id="926b7-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="926b7-108">属性</span><span class="sxs-lookup"><span data-stu-id="926b7-108">Properties</span></span>
|<span data-ttu-id="926b7-109">属性</span><span class="sxs-lookup"><span data-stu-id="926b7-109">Property</span></span>|<span data-ttu-id="926b7-110">类型</span><span class="sxs-lookup"><span data-stu-id="926b7-110">Type</span></span>|<span data-ttu-id="926b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="926b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="926b7-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="926b7-112">succeededUserCount</span></span>|<span data-ttu-id="926b7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="926b7-113">Int32</span></span>|<span data-ttu-id="926b7-114">最近 3 个月用户签入成功总数。</span><span class="sxs-lookup"><span data-stu-id="926b7-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="926b7-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="926b7-115">failedUserCount</span></span>|<span data-ttu-id="926b7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="926b7-116">Int32</span></span>|<span data-ttu-id="926b7-117">最近 3 个月内用户签入失败总数。</span><span class="sxs-lookup"><span data-stu-id="926b7-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="926b7-118">关系</span><span class="sxs-lookup"><span data-stu-id="926b7-118">Relationships</span></span>
<span data-ttu-id="926b7-119">无</span><span class="sxs-lookup"><span data-stu-id="926b7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="926b7-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="926b7-120">JSON Representation</span></span>
<span data-ttu-id="926b7-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="926b7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```




