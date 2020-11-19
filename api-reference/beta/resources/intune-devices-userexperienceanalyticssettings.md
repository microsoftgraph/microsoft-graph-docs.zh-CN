---
title: userExperienceAnalyticsSettings 资源类型
description: 用户体验分析见解是改进用户体验分析分数的建议。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38ef61cf5204b41aa0507bf164e6e8abf0508d90
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259975"
---
# <a name="userexperienceanalyticssettings-resource-type"></a><span data-ttu-id="b36f1-103">userExperienceAnalyticsSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b36f1-103">userExperienceAnalyticsSettings resource type</span></span>

<span data-ttu-id="b36f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b36f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b36f1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b36f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b36f1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b36f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b36f1-107">用户体验分析见解是改进用户体验分析分数的建议。</span><span class="sxs-lookup"><span data-stu-id="b36f1-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="b36f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="b36f1-108">Properties</span></span>
|<span data-ttu-id="b36f1-109">属性</span><span class="sxs-lookup"><span data-stu-id="b36f1-109">Property</span></span>|<span data-ttu-id="b36f1-110">类型</span><span class="sxs-lookup"><span data-stu-id="b36f1-110">Type</span></span>|<span data-ttu-id="b36f1-111">描述</span><span class="sxs-lookup"><span data-stu-id="b36f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b36f1-112">configurationManagerDataConnectorConfigured</span><span class="sxs-lookup"><span data-stu-id="b36f1-112">configurationManagerDataConnectorConfigured</span></span>|<span data-ttu-id="b36f1-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="b36f1-113">Boolean</span></span>|<span data-ttu-id="b36f1-114">如果配置租户附加，则为 True。</span><span class="sxs-lookup"><span data-stu-id="b36f1-114">True if Tenant attach is configured.</span></span> <span data-ttu-id="b36f1-115">如果已配置，则 SCCM 租户附加设备将显示在 UXA 报告中。</span><span class="sxs-lookup"><span data-stu-id="b36f1-115">If configured then SCCM tenant attached devices will show up in UXA reporting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b36f1-116">关系</span><span class="sxs-lookup"><span data-stu-id="b36f1-116">Relationships</span></span>
<span data-ttu-id="b36f1-117">无</span><span class="sxs-lookup"><span data-stu-id="b36f1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b36f1-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b36f1-118">JSON Representation</span></span>
<span data-ttu-id="b36f1-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b36f1-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsSettings",
  "configurationManagerDataConnectorConfigured": true
}
```




