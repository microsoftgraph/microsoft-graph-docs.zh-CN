---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office 客户端配置 AAD 组工作分配目标。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9d59a6adc5478d619187e5414ac92170cbdedd49
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926377"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="f07d4-103">officeConfigurationGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="f07d4-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="f07d4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f07d4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f07d4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f07d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f07d4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f07d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f07d4-107">Office 客户端配置 AAD 组工作分配目标。</span><span class="sxs-lookup"><span data-stu-id="f07d4-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="f07d4-108">继承自[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="f07d4-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f07d4-109">属性</span><span class="sxs-lookup"><span data-stu-id="f07d4-109">Properties</span></span>
|<span data-ttu-id="f07d4-110">属性</span><span class="sxs-lookup"><span data-stu-id="f07d4-110">Property</span></span>|<span data-ttu-id="f07d4-111">类型</span><span class="sxs-lookup"><span data-stu-id="f07d4-111">Type</span></span>|<span data-ttu-id="f07d4-112">说明</span><span class="sxs-lookup"><span data-stu-id="f07d4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f07d4-113">groupId</span><span class="sxs-lookup"><span data-stu-id="f07d4-113">groupId</span></span>|<span data-ttu-id="f07d4-114">字符串</span><span class="sxs-lookup"><span data-stu-id="f07d4-114">String</span></span>|<span data-ttu-id="f07d4-115">AAD 组 Id 目标到该设备的配置。</span><span class="sxs-lookup"><span data-stu-id="f07d4-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f07d4-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="f07d4-116">Relationships</span></span>
<span data-ttu-id="f07d4-117">无</span><span class="sxs-lookup"><span data-stu-id="f07d4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f07d4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f07d4-118">JSON Representation</span></span>
<span data-ttu-id="f07d4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f07d4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



