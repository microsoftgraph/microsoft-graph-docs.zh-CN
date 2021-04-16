---
title: deviceManagementConfigurationSimpleSettingValueTemplate 资源类型
description: 简单设置值模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c4beee60b557449ad6c7af20c10fd98fe859a557
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868419"
---
# <a name="devicemanagementconfigurationsimplesettingvaluetemplate-resource-type"></a><span data-ttu-id="8fb4d-103">deviceManagementConfigurationSimpleSettingValueTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fb4d-103">deviceManagementConfigurationSimpleSettingValueTemplate resource type</span></span>

<span data-ttu-id="8fb4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fb4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fb4d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8fb4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fb4d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8fb4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fb4d-107">简单设置值模板</span><span class="sxs-lookup"><span data-stu-id="8fb4d-107">Simple Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="8fb4d-108">属性</span><span class="sxs-lookup"><span data-stu-id="8fb4d-108">Properties</span></span>
|<span data-ttu-id="8fb4d-109">属性</span><span class="sxs-lookup"><span data-stu-id="8fb4d-109">Property</span></span>|<span data-ttu-id="8fb4d-110">类型</span><span class="sxs-lookup"><span data-stu-id="8fb4d-110">Type</span></span>|<span data-ttu-id="8fb4d-111">说明</span><span class="sxs-lookup"><span data-stu-id="8fb4d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fb4d-112">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="8fb4d-112">settingValueTemplateId</span></span>|<span data-ttu-id="8fb4d-113">String</span><span class="sxs-lookup"><span data-stu-id="8fb4d-113">String</span></span>|<span data-ttu-id="8fb4d-114">设置值模板 ID</span><span class="sxs-lookup"><span data-stu-id="8fb4d-114">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fb4d-115">关系</span><span class="sxs-lookup"><span data-stu-id="8fb4d-115">Relationships</span></span>
<span data-ttu-id="8fb4d-116">无</span><span class="sxs-lookup"><span data-stu-id="8fb4d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fb4d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fb4d-117">JSON Representation</span></span>
<span data-ttu-id="8fb4d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fb4d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
  "settingValueTemplateId": "String"
}
```




