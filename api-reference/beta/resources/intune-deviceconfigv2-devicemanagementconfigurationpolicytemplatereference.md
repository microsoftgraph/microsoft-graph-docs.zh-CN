---
title: deviceManagementConfigurationPolicyTemplateReference 资源类型
description: 策略模板参考信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff61ac1e881ec6bb40750d9cb43d80c6722dd79e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666497"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a><span data-ttu-id="ad9c5-103">deviceManagementConfigurationPolicyTemplateReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad9c5-103">deviceManagementConfigurationPolicyTemplateReference resource type</span></span>

<span data-ttu-id="ad9c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad9c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad9c5-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad9c5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad9c5-107">策略模板参考信息</span><span class="sxs-lookup"><span data-stu-id="ad9c5-107">Policy template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="ad9c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad9c5-108">Properties</span></span>
|<span data-ttu-id="ad9c5-109">属性</span><span class="sxs-lookup"><span data-stu-id="ad9c5-109">Property</span></span>|<span data-ttu-id="ad9c5-110">类型</span><span class="sxs-lookup"><span data-stu-id="ad9c5-110">Type</span></span>|<span data-ttu-id="ad9c5-111">说明</span><span class="sxs-lookup"><span data-stu-id="ad9c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad9c5-112">templateId</span><span class="sxs-lookup"><span data-stu-id="ad9c5-112">templateId</span></span>|<span data-ttu-id="ad9c5-113">String</span><span class="sxs-lookup"><span data-stu-id="ad9c5-113">String</span></span>|<span data-ttu-id="ad9c5-114">模板 ID</span><span class="sxs-lookup"><span data-stu-id="ad9c5-114">Template id</span></span>|
|<span data-ttu-id="ad9c5-115">templateFamily</span><span class="sxs-lookup"><span data-stu-id="ad9c5-115">templateFamily</span></span>|[<span data-ttu-id="ad9c5-116">deviceManagementConfigurationTemplateFamily</span><span class="sxs-lookup"><span data-stu-id="ad9c5-116">deviceManagementConfigurationTemplateFamily</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|<span data-ttu-id="ad9c5-117">引用的模板的模板系列。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-117">Template Family of the referenced Template.</span></span> <span data-ttu-id="ad9c5-118">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-118">This property is read-only.</span></span> <span data-ttu-id="ad9c5-119">可取值为：`none`、`endpointSecurityAntivirus`、`endpointSecurityDiskEncryption`、`endpointSecurityFirewall`、`endpointSecurityEndpointDetectionAndResponse`、`endpointSecurityAttackSurfaceReduction`、`endpointSecurityAccountProtection`、`endpointSecurityApplicationControl`。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-119">Possible values are: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.</span></span>|
|<span data-ttu-id="ad9c5-120">templateDisplayName</span><span class="sxs-lookup"><span data-stu-id="ad9c5-120">templateDisplayName</span></span>|<span data-ttu-id="ad9c5-121">String</span><span class="sxs-lookup"><span data-stu-id="ad9c5-121">String</span></span>|<span data-ttu-id="ad9c5-122">模板显示 引用的模板的名称。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-122">Template Display Name of the referenced template.</span></span> <span data-ttu-id="ad9c5-123">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-123">This property is read-only.</span></span>|
|<span data-ttu-id="ad9c5-124">templateDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="ad9c5-124">templateDisplayVersion</span></span>|<span data-ttu-id="ad9c5-125">String</span><span class="sxs-lookup"><span data-stu-id="ad9c5-125">String</span></span>|<span data-ttu-id="ad9c5-126">模板显示 引用的模板的版本。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-126">Template Display Version of the referenced Template.</span></span> <span data-ttu-id="ad9c5-127">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-127">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad9c5-128">关系</span><span class="sxs-lookup"><span data-stu-id="ad9c5-128">Relationships</span></span>
<span data-ttu-id="ad9c5-129">无</span><span class="sxs-lookup"><span data-stu-id="ad9c5-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad9c5-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad9c5-130">JSON Representation</span></span>
<span data-ttu-id="ad9c5-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad9c5-131">Here is a JSON representation of the resource.</span></span>
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




