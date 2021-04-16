---
title: deviceManagementConfigurationSettingInstanceTemplate 资源类型
description: 设置实例模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76d8c9b985a3ca30f0d2a0a4144128d0e7a1baff
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868451"
---
# <a name="devicemanagementconfigurationsettinginstancetemplate-resource-type"></a><span data-ttu-id="dba65-103">deviceManagementConfigurationSettingInstanceTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="dba65-103">deviceManagementConfigurationSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="dba65-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dba65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dba65-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dba65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dba65-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dba65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dba65-107">设置实例模板</span><span class="sxs-lookup"><span data-stu-id="dba65-107">Setting Instance Template</span></span>

## <a name="properties"></a><span data-ttu-id="dba65-108">属性</span><span class="sxs-lookup"><span data-stu-id="dba65-108">Properties</span></span>
|<span data-ttu-id="dba65-109">属性</span><span class="sxs-lookup"><span data-stu-id="dba65-109">Property</span></span>|<span data-ttu-id="dba65-110">类型</span><span class="sxs-lookup"><span data-stu-id="dba65-110">Type</span></span>|<span data-ttu-id="dba65-111">说明</span><span class="sxs-lookup"><span data-stu-id="dba65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dba65-112">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="dba65-112">settingInstanceTemplateId</span></span>|<span data-ttu-id="dba65-113">String</span><span class="sxs-lookup"><span data-stu-id="dba65-113">String</span></span>|<span data-ttu-id="dba65-114">设置实例模板 ID</span><span class="sxs-lookup"><span data-stu-id="dba65-114">Setting Instance Template Id</span></span>|
|<span data-ttu-id="dba65-115">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dba65-115">settingDefinitionId</span></span>|<span data-ttu-id="dba65-116">String</span><span class="sxs-lookup"><span data-stu-id="dba65-116">String</span></span>|<span data-ttu-id="dba65-117">设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="dba65-117">Setting Definition Id</span></span>|
|<span data-ttu-id="dba65-118">isRequired</span><span class="sxs-lookup"><span data-stu-id="dba65-118">isRequired</span></span>|<span data-ttu-id="dba65-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="dba65-119">Boolean</span></span>|<span data-ttu-id="dba65-120">指示策略是否必须指定此设置。</span><span class="sxs-lookup"><span data-stu-id="dba65-120">Indicates if a policy must specify this setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dba65-121">关系</span><span class="sxs-lookup"><span data-stu-id="dba65-121">Relationships</span></span>
<span data-ttu-id="dba65-122">无</span><span class="sxs-lookup"><span data-stu-id="dba65-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dba65-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dba65-123">JSON Representation</span></span>
<span data-ttu-id="dba65-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dba65-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true
}
```




