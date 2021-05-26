---
title: deviceManagementConfigurationSettingValue 资源类型
description: 设置值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 882946dbcf9440ceacc37a1c843f169ed9e2b1a0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666238"
---
# <a name="devicemanagementconfigurationsettingvalue-resource-type"></a><span data-ttu-id="8eaa4-103">deviceManagementConfigurationSettingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="8eaa4-103">deviceManagementConfigurationSettingValue resource type</span></span>

<span data-ttu-id="8eaa4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eaa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8eaa4-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8eaa4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eaa4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8eaa4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eaa4-107">设置值</span><span class="sxs-lookup"><span data-stu-id="8eaa4-107">Setting value</span></span>

## <a name="properties"></a><span data-ttu-id="8eaa4-108">属性</span><span class="sxs-lookup"><span data-stu-id="8eaa4-108">Properties</span></span>
|<span data-ttu-id="8eaa4-109">属性</span><span class="sxs-lookup"><span data-stu-id="8eaa4-109">Property</span></span>|<span data-ttu-id="8eaa4-110">类型</span><span class="sxs-lookup"><span data-stu-id="8eaa4-110">Type</span></span>|<span data-ttu-id="8eaa4-111">说明</span><span class="sxs-lookup"><span data-stu-id="8eaa4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eaa4-112">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="8eaa4-112">settingValueTemplateReference</span></span>|[<span data-ttu-id="8eaa4-113">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="8eaa4-113">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="8eaa4-114">设置值模板引用</span><span class="sxs-lookup"><span data-stu-id="8eaa4-114">Setting value template reference</span></span>|

## <a name="relationships"></a><span data-ttu-id="8eaa4-115">关系</span><span class="sxs-lookup"><span data-stu-id="8eaa4-115">Relationships</span></span>
<span data-ttu-id="8eaa4-116">无</span><span class="sxs-lookup"><span data-stu-id="8eaa4-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8eaa4-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8eaa4-117">JSON Representation</span></span>
<span data-ttu-id="8eaa4-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8eaa4-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  }
}
```




