---
title: suggestedEnrollmentLimit 资源类型
description: 当给定注册类型时，suggestedEnrollmentLimit 资源表示建议的注册限制。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99efb75bcf52b841dcf67741045b7207a85eb3cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081987"
---
# <a name="suggestedenrollmentlimit-resource-type"></a><span data-ttu-id="7be91-103">suggestedEnrollmentLimit 资源类型</span><span class="sxs-lookup"><span data-stu-id="7be91-103">suggestedEnrollmentLimit resource type</span></span>

<span data-ttu-id="7be91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7be91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7be91-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7be91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7be91-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7be91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7be91-107">当给定注册类型时，suggestedEnrollmentLimit 资源表示建议的注册限制。</span><span class="sxs-lookup"><span data-stu-id="7be91-107">The suggestedEnrollmentLimit resource represents the suggested enrollment limit when given an enrollment type.</span></span>

## <a name="properties"></a><span data-ttu-id="7be91-108">属性</span><span class="sxs-lookup"><span data-stu-id="7be91-108">Properties</span></span>
|<span data-ttu-id="7be91-109">属性</span><span class="sxs-lookup"><span data-stu-id="7be91-109">Property</span></span>|<span data-ttu-id="7be91-110">类型</span><span class="sxs-lookup"><span data-stu-id="7be91-110">Type</span></span>|<span data-ttu-id="7be91-111">说明</span><span class="sxs-lookup"><span data-stu-id="7be91-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7be91-112">suggestedDailyLimit</span><span class="sxs-lookup"><span data-stu-id="7be91-112">suggestedDailyLimit</span></span>|<span data-ttu-id="7be91-113">Int32</span><span class="sxs-lookup"><span data-stu-id="7be91-113">Int32</span></span>|<span data-ttu-id="7be91-114">一天内建议的登记限制</span><span class="sxs-lookup"><span data-stu-id="7be91-114">The suggested enrollment limit within a day</span></span>|

## <a name="relationships"></a><span data-ttu-id="7be91-115">关系</span><span class="sxs-lookup"><span data-stu-id="7be91-115">Relationships</span></span>
<span data-ttu-id="7be91-116">无</span><span class="sxs-lookup"><span data-stu-id="7be91-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7be91-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7be91-117">JSON Representation</span></span>
<span data-ttu-id="7be91-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7be91-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.suggestedEnrollmentLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.suggestedEnrollmentLimit",
  "suggestedDailyLimit": 1024
}
```






