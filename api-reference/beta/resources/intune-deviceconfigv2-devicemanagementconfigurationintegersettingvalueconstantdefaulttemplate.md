---
title: deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate 资源类型
description: 整数设置值常量默认模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8570f0b5c2b0059d0ad991d637592e081327e452
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666847"
---
# <a name="devicemanagementconfigurationintegersettingvalueconstantdefaulttemplate-resource-type"></a><span data-ttu-id="8a6be-103">deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a6be-103">deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate resource type</span></span>

<span data-ttu-id="8a6be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a6be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a6be-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8a6be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a6be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a6be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a6be-107">整数设置值常量默认模板</span><span class="sxs-lookup"><span data-stu-id="8a6be-107">Integer Setting Value Constant Default Template</span></span>


<span data-ttu-id="8a6be-108">继承自 [deviceManagementConfigurationIntegerSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)</span><span class="sxs-lookup"><span data-stu-id="8a6be-108">Inherits from [deviceManagementConfigurationIntegerSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationintegersettingvaluedefaulttemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8a6be-109">属性</span><span class="sxs-lookup"><span data-stu-id="8a6be-109">Properties</span></span>
|<span data-ttu-id="8a6be-110">属性</span><span class="sxs-lookup"><span data-stu-id="8a6be-110">Property</span></span>|<span data-ttu-id="8a6be-111">类型</span><span class="sxs-lookup"><span data-stu-id="8a6be-111">Type</span></span>|<span data-ttu-id="8a6be-112">说明</span><span class="sxs-lookup"><span data-stu-id="8a6be-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a6be-113">constantValue</span><span class="sxs-lookup"><span data-stu-id="8a6be-113">constantValue</span></span>|<span data-ttu-id="8a6be-114">Int32</span><span class="sxs-lookup"><span data-stu-id="8a6be-114">Int32</span></span>|<span data-ttu-id="8a6be-115">默认常量值。</span><span class="sxs-lookup"><span data-stu-id="8a6be-115">Default Constant Value.</span></span> <span data-ttu-id="8a6be-116">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="8a6be-116">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a6be-117">关系</span><span class="sxs-lookup"><span data-stu-id="8a6be-117">Relationships</span></span>
<span data-ttu-id="8a6be-118">无</span><span class="sxs-lookup"><span data-stu-id="8a6be-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a6be-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a6be-119">JSON Representation</span></span>
<span data-ttu-id="8a6be-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a6be-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueConstantDefaultTemplate",
  "constantValue": 1024
}
```




