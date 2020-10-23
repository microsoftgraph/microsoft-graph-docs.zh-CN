---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office 客户端配置 AAD 组分配目标。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bcfb80008880f6e2cd15119a3dda796a37a18250
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723969"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="2304c-103">officeConfigurationGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="2304c-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="2304c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2304c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2304c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2304c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2304c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2304c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2304c-107">Office 客户端配置 AAD 组分配目标。</span><span class="sxs-lookup"><span data-stu-id="2304c-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="2304c-108">继承自 [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="2304c-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2304c-109">属性</span><span class="sxs-lookup"><span data-stu-id="2304c-109">Properties</span></span>
|<span data-ttu-id="2304c-110">属性</span><span class="sxs-lookup"><span data-stu-id="2304c-110">Property</span></span>|<span data-ttu-id="2304c-111">类型</span><span class="sxs-lookup"><span data-stu-id="2304c-111">Type</span></span>|<span data-ttu-id="2304c-112">说明</span><span class="sxs-lookup"><span data-stu-id="2304c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2304c-113">groupId</span><span class="sxs-lookup"><span data-stu-id="2304c-113">groupId</span></span>|<span data-ttu-id="2304c-114">String</span><span class="sxs-lookup"><span data-stu-id="2304c-114">String</span></span>|<span data-ttu-id="2304c-115">要将设备配置定向到的 AAD 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="2304c-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2304c-116">关系</span><span class="sxs-lookup"><span data-stu-id="2304c-116">Relationships</span></span>
<span data-ttu-id="2304c-117">无</span><span class="sxs-lookup"><span data-stu-id="2304c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2304c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2304c-118">JSON Representation</span></span>
<span data-ttu-id="2304c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2304c-119">Here is a JSON representation of the resource.</span></span>
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





