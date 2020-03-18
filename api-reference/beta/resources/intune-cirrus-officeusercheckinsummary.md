---
title: officeUserCheckinSummary 资源类型
description: 描述租户签入统计信息的实体。
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9ef202194c8817e500d27a96ae3dbf4e5e1a8359
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797295"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="a6679-103">officeUserCheckinSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6679-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="a6679-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a6679-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6679-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6679-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6679-106">描述租户签入统计信息的实体。</span><span class="sxs-lookup"><span data-stu-id="a6679-106">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="a6679-107">属性</span><span class="sxs-lookup"><span data-stu-id="a6679-107">Properties</span></span>
|<span data-ttu-id="a6679-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6679-108">Property</span></span>|<span data-ttu-id="a6679-109">类型</span><span class="sxs-lookup"><span data-stu-id="a6679-109">Type</span></span>|<span data-ttu-id="a6679-110">说明</span><span class="sxs-lookup"><span data-stu-id="a6679-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6679-111">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="a6679-111">succeededUserCount</span></span>|<span data-ttu-id="a6679-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a6679-112">Int32</span></span>|<span data-ttu-id="a6679-113">最近3个月内成功的用户签入次数总计。</span><span class="sxs-lookup"><span data-stu-id="a6679-113">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="a6679-114">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="a6679-114">failedUserCount</span></span>|<span data-ttu-id="a6679-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a6679-115">Int32</span></span>|<span data-ttu-id="a6679-116">最近3个月的用户签入失败总计。</span><span class="sxs-lookup"><span data-stu-id="a6679-116">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6679-117">关系</span><span class="sxs-lookup"><span data-stu-id="a6679-117">Relationships</span></span>
<span data-ttu-id="a6679-118">无</span><span class="sxs-lookup"><span data-stu-id="a6679-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6679-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6679-119">JSON Representation</span></span>
<span data-ttu-id="a6679-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6679-120">Here is a JSON representation of the resource.</span></span>
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



