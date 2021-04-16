---
title: deviceManagementConfigurationPolicyTemplateReference 资源类型
description: 策略模板参考信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dee3cf25ed42f2c1ecdbf824fd807ed00c8ce91b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868426"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a><span data-ttu-id="7b94a-103">deviceManagementConfigurationPolicyTemplateReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b94a-103">deviceManagementConfigurationPolicyTemplateReference resource type</span></span>

<span data-ttu-id="7b94a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b94a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7b94a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7b94a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b94a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7b94a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b94a-107">策略模板参考信息</span><span class="sxs-lookup"><span data-stu-id="7b94a-107">Policy template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="7b94a-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b94a-108">Properties</span></span>
|<span data-ttu-id="7b94a-109">属性</span><span class="sxs-lookup"><span data-stu-id="7b94a-109">Property</span></span>|<span data-ttu-id="7b94a-110">类型</span><span class="sxs-lookup"><span data-stu-id="7b94a-110">Type</span></span>|<span data-ttu-id="7b94a-111">说明</span><span class="sxs-lookup"><span data-stu-id="7b94a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b94a-112">templateId</span><span class="sxs-lookup"><span data-stu-id="7b94a-112">templateId</span></span>|<span data-ttu-id="7b94a-113">String</span><span class="sxs-lookup"><span data-stu-id="7b94a-113">String</span></span>|<span data-ttu-id="7b94a-114">模板 ID</span><span class="sxs-lookup"><span data-stu-id="7b94a-114">Template id</span></span>|
|<span data-ttu-id="7b94a-115">templateFamily</span><span class="sxs-lookup"><span data-stu-id="7b94a-115">templateFamily</span></span>|[<span data-ttu-id="7b94a-116">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="7b94a-116">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="7b94a-117">引用的模板的模板系列。</span><span class="sxs-lookup"><span data-stu-id="7b94a-117">Template Family of the referenced Template.</span></span> <span data-ttu-id="7b94a-118">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7b94a-118">This property is read-only.</span></span> <span data-ttu-id="7b94a-119">可取值为：`none`、`endpointSecurityAntivirus`、`endpointSecurityDiskEncryption`、`endpointSecurityFirewall`、`endpointSecurityEndpointDectionAndResponse`、`endpointSecurityAttackSurfaceReduction`、`endpointSecurityAccountProtection`、`endpointSecurityApplicationControl`。</span><span class="sxs-lookup"><span data-stu-id="7b94a-119">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="7b94a-120">templateDisplayName</span><span class="sxs-lookup"><span data-stu-id="7b94a-120">templateDisplayName</span></span>|<span data-ttu-id="7b94a-121">String</span><span class="sxs-lookup"><span data-stu-id="7b94a-121">String</span></span>|<span data-ttu-id="7b94a-122">模板显示 引用的模板的名称。</span><span class="sxs-lookup"><span data-stu-id="7b94a-122">Template Display Name of the referenced template.</span></span> <span data-ttu-id="7b94a-123">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7b94a-123">This property is read-only.</span></span>|
|<span data-ttu-id="7b94a-124">templateDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="7b94a-124">templateDisplayVersion</span></span>|<span data-ttu-id="7b94a-125">String</span><span class="sxs-lookup"><span data-stu-id="7b94a-125">String</span></span>|<span data-ttu-id="7b94a-126">模板显示 引用的模板的版本。</span><span class="sxs-lookup"><span data-stu-id="7b94a-126">Template Display Version of the referenced Template.</span></span> <span data-ttu-id="7b94a-127">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7b94a-127">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b94a-128">关系</span><span class="sxs-lookup"><span data-stu-id="7b94a-128">Relationships</span></span>
<span data-ttu-id="7b94a-129">无</span><span class="sxs-lookup"><span data-stu-id="7b94a-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b94a-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b94a-130">JSON Representation</span></span>
<span data-ttu-id="7b94a-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b94a-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
  "templateId": "String",
  "templateFamily": "String",
  "templateDisplayName": "String",
  "templateDisplayVersion": "String"
}
```




