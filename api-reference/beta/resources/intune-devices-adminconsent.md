---
title: adminConsent 资源类型
description: 管理员同意信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11a8cd99c544dcd11b713d4c3c98eede77c48eb1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209218"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="7ef81-103">adminConsent 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ef81-103">adminConsent resource type</span></span>

<span data-ttu-id="7ef81-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ef81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ef81-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ef81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ef81-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ef81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ef81-107">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="7ef81-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="7ef81-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ef81-108">Properties</span></span>
|<span data-ttu-id="7ef81-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ef81-109">Property</span></span>|<span data-ttu-id="7ef81-110">类型</span><span class="sxs-lookup"><span data-stu-id="7ef81-110">Type</span></span>|<span data-ttu-id="7ef81-111">说明</span><span class="sxs-lookup"><span data-stu-id="7ef81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ef81-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="7ef81-112">shareAPNSData</span></span>|[<span data-ttu-id="7ef81-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="7ef81-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="7ef81-114">将用户和设备数据共享到 Apple 的管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="7ef81-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="7ef81-115">可取值为：`notConfigured`、`granted`、`notGranted`。</span><span class="sxs-lookup"><span data-stu-id="7ef81-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="7ef81-116">shareUserExperienceAnalyticsData</span><span class="sxs-lookup"><span data-stu-id="7ef81-116">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="7ef81-117">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="7ef81-117">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="7ef81-118">获取或设置用于共享用户体验分析数据的管理员同意。</span><span class="sxs-lookup"><span data-stu-id="7ef81-118">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="7ef81-119">可取值为：`notConfigured`、`granted`、`notGranted`。</span><span class="sxs-lookup"><span data-stu-id="7ef81-119">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ef81-120">关系</span><span class="sxs-lookup"><span data-stu-id="7ef81-120">Relationships</span></span>
<span data-ttu-id="7ef81-121">无</span><span class="sxs-lookup"><span data-stu-id="7ef81-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ef81-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ef81-122">JSON Representation</span></span>
<span data-ttu-id="7ef81-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ef81-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```




