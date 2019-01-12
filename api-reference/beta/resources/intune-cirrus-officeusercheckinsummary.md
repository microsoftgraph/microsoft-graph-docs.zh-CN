---
title: officeUserCheckinSummary 资源类型
description: 介绍租户中签入 stats 的实体。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 374f5113a517b52ae7af6381f575ac60e5d00ae4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946579"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="f5825-103">officeUserCheckinSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5825-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="f5825-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f5825-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5825-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f5825-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5825-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f5825-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5825-107">介绍租户中签入 stats 的实体。</span><span class="sxs-lookup"><span data-stu-id="f5825-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="f5825-108">属性</span><span class="sxs-lookup"><span data-stu-id="f5825-108">Properties</span></span>
|<span data-ttu-id="f5825-109">属性</span><span class="sxs-lookup"><span data-stu-id="f5825-109">Property</span></span>|<span data-ttu-id="f5825-110">类型</span><span class="sxs-lookup"><span data-stu-id="f5825-110">Type</span></span>|<span data-ttu-id="f5825-111">说明</span><span class="sxs-lookup"><span data-stu-id="f5825-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5825-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="f5825-112">succeededUserCount</span></span>|<span data-ttu-id="f5825-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f5825-113">Int32</span></span>|<span data-ttu-id="f5825-114">总用户成功检查的最近 3 个月的项。</span><span class="sxs-lookup"><span data-stu-id="f5825-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="f5825-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="f5825-115">failedUserCount</span></span>|<span data-ttu-id="f5825-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f5825-116">Int32</span></span>|<span data-ttu-id="f5825-117">失败的总用户检查的最近 3 个月的项。</span><span class="sxs-lookup"><span data-stu-id="f5825-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5825-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="f5825-118">Relationships</span></span>
<span data-ttu-id="f5825-119">无</span><span class="sxs-lookup"><span data-stu-id="f5825-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f5825-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5825-120">JSON Representation</span></span>
<span data-ttu-id="f5825-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5825-121">Here is a JSON representation of the resource.</span></span>
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



