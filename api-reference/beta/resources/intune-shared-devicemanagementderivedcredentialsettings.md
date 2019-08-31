---
title: deviceManagementDerivedCredentialSettings 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8cbf9ae512659459035faf5938e3eae2dd2f09d3
ms.sourcegitcommit: 0f3e0bd7b57870a0f7b34cf52eaf4776ac82671e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2019
ms.locfileid: "36699535"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a><span data-ttu-id="649c5-103">deviceManagementDerivedCredentialSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="649c5-103">deviceManagementDerivedCredentialSettings resource type</span></span>

> <span data-ttu-id="649c5-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="649c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="649c5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="649c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="649c5-106">DeviceManagementDerivedCredentialSettings 资源代表其内容因工作流而异的容器, 包括:</span><span class="sxs-lookup"><span data-stu-id="649c5-106">The deviceManagementDerivedCredentialSettings resource represents a container whose contents vary according to workflow, including:</span></span>  

- <span data-ttu-id="649c5-107">设备配置设置</span><span class="sxs-lookup"><span data-stu-id="649c5-107">Device configuration settings</span></span>
- <span data-ttu-id="649c5-108">RA 策略</span><span class="sxs-lookup"><span data-stu-id="649c5-108">RA Policy</span></span>

## <a name="methods"></a><span data-ttu-id="649c5-109">方法</span><span class="sxs-lookup"><span data-stu-id="649c5-109">Methods</span></span>
|<span data-ttu-id="649c5-110">方法</span><span class="sxs-lookup"><span data-stu-id="649c5-110">Method</span></span>|<span data-ttu-id="649c5-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="649c5-111">Return Type</span></span>|<span data-ttu-id="649c5-112">说明</span><span class="sxs-lookup"><span data-stu-id="649c5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="649c5-113">获取 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="649c5-113">Get deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-get.md)|[<span data-ttu-id="649c5-114">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="649c5-114">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="649c5-115">读取[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="649c5-115">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="649c5-116">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="649c5-116">Update deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-update.md)|[<span data-ttu-id="649c5-117">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="649c5-117">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="649c5-118">更新[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="649c5-118">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|<span data-ttu-id="649c5-119">**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="649c5-119">**Resource Access Policy**</span></span>|
|[<span data-ttu-id="649c5-120">列出 deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="649c5-120">List deviceManagementDerivedCredentialSettingses</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-list.md)|<span data-ttu-id="649c5-121">[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)集合</span><span class="sxs-lookup"><span data-stu-id="649c5-121">[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) collection</span></span>|<span data-ttu-id="649c5-122">列出[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="649c5-122">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>|
|[<span data-ttu-id="649c5-123">创建 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="649c5-123">Create deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-create.md)|[<span data-ttu-id="649c5-124">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="649c5-124">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="649c5-125">创建新的[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="649c5-125">Create a new [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="649c5-126">删除 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="649c5-126">Delete deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-delete.md)|<span data-ttu-id="649c5-127">无</span><span class="sxs-lookup"><span data-stu-id="649c5-127">None</span></span>|<span data-ttu-id="649c5-128">删除[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="649c5-128">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>|


## <a name="properties"></a><span data-ttu-id="649c5-129">属性</span><span class="sxs-lookup"><span data-stu-id="649c5-129">Properties</span></span>
|<span data-ttu-id="649c5-130">属性</span><span class="sxs-lookup"><span data-stu-id="649c5-130">Property</span></span>|<span data-ttu-id="649c5-131">类型</span><span class="sxs-lookup"><span data-stu-id="649c5-131">Type</span></span>|<span data-ttu-id="649c5-132">说明</span><span class="sxs-lookup"><span data-stu-id="649c5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="649c5-133">id</span><span class="sxs-lookup"><span data-stu-id="649c5-133">id</span></span>|<span data-ttu-id="649c5-134">String</span><span class="sxs-lookup"><span data-stu-id="649c5-134">String</span></span>|<span data-ttu-id="649c5-135">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="649c5-135">Unique identifier for the Derived Credential</span></span>|

## <a name="relationships"></a><span data-ttu-id="649c5-136">关系</span><span class="sxs-lookup"><span data-stu-id="649c5-136">Relationships</span></span>
<span data-ttu-id="649c5-137">无</span><span class="sxs-lookup"><span data-stu-id="649c5-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="649c5-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="649c5-138">JSON Representation</span></span>
<span data-ttu-id="649c5-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="649c5-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDerivedCredentialSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "String (identifier)"
}
```



