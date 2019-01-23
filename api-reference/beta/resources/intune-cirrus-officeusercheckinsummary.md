---
title: officeUserCheckinSummary 资源类型
description: 介绍租户中签入 stats 的实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d44c978ff1442c98038bf627397de5ca3a0ca3bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411006"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="f6bf2-103">officeUserCheckinSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6bf2-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="f6bf2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f6bf2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f6bf2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f6bf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6bf2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6bf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6bf2-107">介绍租户中签入 stats 的实体。</span><span class="sxs-lookup"><span data-stu-id="f6bf2-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="f6bf2-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6bf2-108">Properties</span></span>
|<span data-ttu-id="f6bf2-109">属性</span><span class="sxs-lookup"><span data-stu-id="f6bf2-109">Property</span></span>|<span data-ttu-id="f6bf2-110">类型</span><span class="sxs-lookup"><span data-stu-id="f6bf2-110">Type</span></span>|<span data-ttu-id="f6bf2-111">说明</span><span class="sxs-lookup"><span data-stu-id="f6bf2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6bf2-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="f6bf2-112">succeededUserCount</span></span>|<span data-ttu-id="f6bf2-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f6bf2-113">Int32</span></span>|<span data-ttu-id="f6bf2-114">总用户成功检查的最近 3 个月的项。</span><span class="sxs-lookup"><span data-stu-id="f6bf2-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="f6bf2-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="f6bf2-115">failedUserCount</span></span>|<span data-ttu-id="f6bf2-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f6bf2-116">Int32</span></span>|<span data-ttu-id="f6bf2-117">失败的总用户检查的最近 3 个月的项。</span><span class="sxs-lookup"><span data-stu-id="f6bf2-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6bf2-118">关系</span><span class="sxs-lookup"><span data-stu-id="f6bf2-118">Relationships</span></span>
<span data-ttu-id="f6bf2-119">无</span><span class="sxs-lookup"><span data-stu-id="f6bf2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6bf2-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6bf2-120">JSON Representation</span></span>
<span data-ttu-id="f6bf2-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6bf2-121">Here is a JSON representation of the resource.</span></span>
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



