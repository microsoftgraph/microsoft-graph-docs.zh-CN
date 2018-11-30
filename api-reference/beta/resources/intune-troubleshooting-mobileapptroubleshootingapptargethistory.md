---
title: mobileAppTroubleshootingAppTargetHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
ms.openlocfilehash: c7397e182c1af4c01753623a655579f5f8c6ee08
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044722"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="ba4a1-103">mobileAppTroubleshootingAppTargetHistory 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba4a1-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="ba4a1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba4a1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba4a1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba4a1-107">移动应用程序疑难解答事件中包含的历史记录项。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="ba4a1-108">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ba4a1-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ba4a1-109">属性</span><span class="sxs-lookup"><span data-stu-id="ba4a1-109">Properties</span></span>
|<span data-ttu-id="ba4a1-110">属性</span><span class="sxs-lookup"><span data-stu-id="ba4a1-110">Property</span></span>|<span data-ttu-id="ba4a1-111">类型</span><span class="sxs-lookup"><span data-stu-id="ba4a1-111">Type</span></span>|<span data-ttu-id="ba4a1-112">说明</span><span class="sxs-lookup"><span data-stu-id="ba4a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba4a1-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="ba4a1-113">occurrenceDateTime</span></span>|<span data-ttu-id="ba4a1-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba4a1-114">DateTimeOffset</span></span>|<span data-ttu-id="ba4a1-115">历史记录项所发生的时间。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-115">Time when the history item occurred.</span></span> <span data-ttu-id="ba4a1-116">继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="ba4a1-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="ba4a1-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="ba4a1-117">securityGroupId</span></span>|<span data-ttu-id="ba4a1-118">字符串</span><span class="sxs-lookup"><span data-stu-id="ba4a1-118">String</span></span>|<span data-ttu-id="ba4a1-119">它已向其目标 AAD 安全组 id。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="ba4a1-120">runState</span><span class="sxs-lookup"><span data-stu-id="ba4a1-120">runState</span></span>|[<span data-ttu-id="ba4a1-121">runState</span><span class="sxs-lookup"><span data-stu-id="ba4a1-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="ba4a1-122">项目的状态。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-122">Status of the item.</span></span> <span data-ttu-id="ba4a1-123">可取值为：`unknown`、`success`、`fail`。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="ba4a1-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="ba4a1-124">errorCode</span></span>|<span data-ttu-id="ba4a1-125">String</span><span class="sxs-lookup"><span data-stu-id="ba4a1-125">String</span></span>|<span data-ttu-id="ba4a1-126">故障，如果没有出现故障空的错误代码。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba4a1-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="ba4a1-127">Relationships</span></span>
<span data-ttu-id="ba4a1-128">无</span><span class="sxs-lookup"><span data-stu-id="ba4a1-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ba4a1-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba4a1-129">JSON Representation</span></span>
<span data-ttu-id="ba4a1-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba4a1-130">Here is a JSON representation of the resource.</span></span>
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





