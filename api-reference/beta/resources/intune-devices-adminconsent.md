---
title: adminConsent 资源类型
description: 管理员同意信息。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0f0f60f39c676fb8c6aca5144b2aa3b561b7cbaf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785173"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="df55c-103">adminConsent 资源类型</span><span class="sxs-lookup"><span data-stu-id="df55c-103">adminConsent resource type</span></span>

> <span data-ttu-id="df55c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df55c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df55c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df55c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df55c-106">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="df55c-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="df55c-107">属性</span><span class="sxs-lookup"><span data-stu-id="df55c-107">Properties</span></span>
|<span data-ttu-id="df55c-108">属性</span><span class="sxs-lookup"><span data-stu-id="df55c-108">Property</span></span>|<span data-ttu-id="df55c-109">类型</span><span class="sxs-lookup"><span data-stu-id="df55c-109">Type</span></span>|<span data-ttu-id="df55c-110">说明</span><span class="sxs-lookup"><span data-stu-id="df55c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df55c-111">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="df55c-111">shareAPNSData</span></span>|[<span data-ttu-id="df55c-112">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="df55c-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="df55c-113">将用户和设备数据共享到 Apple 的管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="df55c-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="df55c-114">可取值为：`notConfigured`、`granted`、`notGranted`。</span><span class="sxs-lookup"><span data-stu-id="df55c-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="df55c-115">shareUserExperienceAnalyticsData</span><span class="sxs-lookup"><span data-stu-id="df55c-115">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="df55c-116">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="df55c-116">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="df55c-117">获取或设置用于共享用户体验分析数据的管理员同意。</span><span class="sxs-lookup"><span data-stu-id="df55c-117">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="df55c-118">可取值为：`notConfigured`、`granted`、`notGranted`。</span><span class="sxs-lookup"><span data-stu-id="df55c-118">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df55c-119">关系</span><span class="sxs-lookup"><span data-stu-id="df55c-119">Relationships</span></span>
<span data-ttu-id="df55c-120">无</span><span class="sxs-lookup"><span data-stu-id="df55c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df55c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df55c-121">JSON Representation</span></span>
<span data-ttu-id="df55c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df55c-122">Here is a JSON representation of the resource.</span></span>
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



