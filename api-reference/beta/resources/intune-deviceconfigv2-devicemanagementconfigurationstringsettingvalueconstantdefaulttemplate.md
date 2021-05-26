---
title: deviceManagementConfigurationStringSettingValueConstantDefaultTemplate 资源类型
description: 字符串设置值常量默认模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5cf9a9ffead755691cbefe12a56d36b4e8b44d40
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666854"
---
# <a name="devicemanagementconfigurationstringsettingvalueconstantdefaulttemplate-resource-type"></a><span data-ttu-id="d4c2e-103">deviceManagementConfigurationStringSettingValueConstantDefaultTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4c2e-103">deviceManagementConfigurationStringSettingValueConstantDefaultTemplate resource type</span></span>

<span data-ttu-id="d4c2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4c2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4c2e-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4c2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4c2e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4c2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4c2e-107">字符串设置值常量默认模板</span><span class="sxs-lookup"><span data-stu-id="d4c2e-107">String Setting Value Constant Default Template</span></span>


<span data-ttu-id="d4c2e-108">继承自 [deviceManagementConfigurationStringSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvaluedefaulttemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d4c2e-108">Inherits from [deviceManagementConfigurationStringSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvaluedefaulttemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4c2e-109">属性</span><span class="sxs-lookup"><span data-stu-id="d4c2e-109">Properties</span></span>
|<span data-ttu-id="d4c2e-110">属性</span><span class="sxs-lookup"><span data-stu-id="d4c2e-110">Property</span></span>|<span data-ttu-id="d4c2e-111">类型</span><span class="sxs-lookup"><span data-stu-id="d4c2e-111">Type</span></span>|<span data-ttu-id="d4c2e-112">说明</span><span class="sxs-lookup"><span data-stu-id="d4c2e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4c2e-113">constantValue</span><span class="sxs-lookup"><span data-stu-id="d4c2e-113">constantValue</span></span>|<span data-ttu-id="d4c2e-114">String</span><span class="sxs-lookup"><span data-stu-id="d4c2e-114">String</span></span>|<span data-ttu-id="d4c2e-115">默认常量值</span><span class="sxs-lookup"><span data-stu-id="d4c2e-115">Default Constant Value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4c2e-116">关系</span><span class="sxs-lookup"><span data-stu-id="d4c2e-116">Relationships</span></span>
<span data-ttu-id="d4c2e-117">无</span><span class="sxs-lookup"><span data-stu-id="d4c2e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4c2e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4c2e-118">JSON Representation</span></span>
<span data-ttu-id="d4c2e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4c2e-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
  "constantValue": "String"
}
```




