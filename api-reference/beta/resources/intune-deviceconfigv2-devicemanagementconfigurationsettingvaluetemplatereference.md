---
title: deviceManagementConfigurationSettingValueTemplateReference 资源类型
description: 设置值模板参考信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa4ecc07044d90bfc869467de8e8249f7581e228
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666831"
---
# <a name="devicemanagementconfigurationsettingvaluetemplatereference-resource-type"></a><span data-ttu-id="0c74e-103">deviceManagementConfigurationSettingValueTemplateReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c74e-103">deviceManagementConfigurationSettingValueTemplateReference resource type</span></span>

<span data-ttu-id="0c74e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c74e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c74e-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0c74e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c74e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c74e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c74e-107">设置值模板参考信息</span><span class="sxs-lookup"><span data-stu-id="0c74e-107">Setting value template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="0c74e-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c74e-108">Properties</span></span>
|<span data-ttu-id="0c74e-109">属性</span><span class="sxs-lookup"><span data-stu-id="0c74e-109">Property</span></span>|<span data-ttu-id="0c74e-110">类型</span><span class="sxs-lookup"><span data-stu-id="0c74e-110">Type</span></span>|<span data-ttu-id="0c74e-111">说明</span><span class="sxs-lookup"><span data-stu-id="0c74e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c74e-112">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="0c74e-112">settingValueTemplateId</span></span>|<span data-ttu-id="0c74e-113">String</span><span class="sxs-lookup"><span data-stu-id="0c74e-113">String</span></span>|<span data-ttu-id="0c74e-114">设置值模板 ID</span><span class="sxs-lookup"><span data-stu-id="0c74e-114">Setting value template id</span></span>|
|<span data-ttu-id="0c74e-115">useTemplateDefault</span><span class="sxs-lookup"><span data-stu-id="0c74e-115">useTemplateDefault</span></span>|<span data-ttu-id="0c74e-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="0c74e-116">Boolean</span></span>|<span data-ttu-id="0c74e-117">指示是否更新策略设置值以匹配模板设置默认值</span><span class="sxs-lookup"><span data-stu-id="0c74e-117">Indicates whether to update policy setting value to match template setting default value</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c74e-118">关系</span><span class="sxs-lookup"><span data-stu-id="0c74e-118">Relationships</span></span>
<span data-ttu-id="0c74e-119">无</span><span class="sxs-lookup"><span data-stu-id="0c74e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c74e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c74e-120">JSON Representation</span></span>
<span data-ttu-id="0c74e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c74e-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
  "settingValueTemplateId": "String",
  "useTemplateDefault": true
}
```




