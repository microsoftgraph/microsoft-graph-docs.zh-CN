---
title: mobileAppTroubleshootingAppTargetHistory 资源类型
description: 移动应用故障排除事件中包含的历史记录项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a19399788462b6dc7cae995971ddb443051b6959
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570706"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="b77c3-103">mobileAppTroubleshootingAppTargetHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="b77c3-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="b77c3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b77c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b77c3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b77c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b77c3-106">移动应用故障排除事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="b77c3-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="b77c3-107">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b77c3-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b77c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="b77c3-108">Properties</span></span>
|<span data-ttu-id="b77c3-109">属性</span><span class="sxs-lookup"><span data-stu-id="b77c3-109">Property</span></span>|<span data-ttu-id="b77c3-110">类型</span><span class="sxs-lookup"><span data-stu-id="b77c3-110">Type</span></span>|<span data-ttu-id="b77c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="b77c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b77c3-112">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="b77c3-112">occurrenceDateTime</span></span>|<span data-ttu-id="b77c3-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b77c3-113">DateTimeOffset</span></span>|<span data-ttu-id="b77c3-114">历史记录项目发生的时间。</span><span class="sxs-lookup"><span data-stu-id="b77c3-114">Time when the history item occurred.</span></span> <span data-ttu-id="b77c3-115">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="b77c3-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="b77c3-116">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="b77c3-116">securityGroupId</span></span>|<span data-ttu-id="b77c3-117">String</span><span class="sxs-lookup"><span data-stu-id="b77c3-117">String</span></span>|<span data-ttu-id="b77c3-118">目标为的 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="b77c3-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="b77c3-119">runState</span><span class="sxs-lookup"><span data-stu-id="b77c3-119">runState</span></span>|[<span data-ttu-id="b77c3-120">runState</span><span class="sxs-lookup"><span data-stu-id="b77c3-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="b77c3-121">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="b77c3-121">Status of the item.</span></span> <span data-ttu-id="b77c3-122">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="b77c3-122">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="b77c3-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="b77c3-123">errorCode</span></span>|<span data-ttu-id="b77c3-124">String</span><span class="sxs-lookup"><span data-stu-id="b77c3-124">String</span></span>|<span data-ttu-id="b77c3-125">失败的错误代码, 如果没有失败, 则为空。</span><span class="sxs-lookup"><span data-stu-id="b77c3-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b77c3-126">关系</span><span class="sxs-lookup"><span data-stu-id="b77c3-126">Relationships</span></span>
<span data-ttu-id="b77c3-127">无</span><span class="sxs-lookup"><span data-stu-id="b77c3-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b77c3-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b77c3-128">JSON Representation</span></span>
<span data-ttu-id="b77c3-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b77c3-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```



