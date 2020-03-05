---
title: deviceManagementDerivedCredentialSettings 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e104ef869f6a033947fe6ffc01144e04c6550a2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523700"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a><span data-ttu-id="8331e-103">deviceManagementDerivedCredentialSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8331e-103">deviceManagementDerivedCredentialSettings resource type</span></span>

<span data-ttu-id="8331e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8331e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8331e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8331e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8331e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8331e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8331e-107">DeviceManagementDerivedCredentialSettings 资源代表其内容因工作流而异的容器，包括：</span><span class="sxs-lookup"><span data-stu-id="8331e-107">The deviceManagementDerivedCredentialSettings resource represents a container whose contents vary according to workflow, including:</span></span>  

- <span data-ttu-id="8331e-108">设备配置设置</span><span class="sxs-lookup"><span data-stu-id="8331e-108">Device configuration settings</span></span>
- <span data-ttu-id="8331e-109">RA 策略</span><span class="sxs-lookup"><span data-stu-id="8331e-109">RA Policy</span></span>

## <a name="methods"></a><span data-ttu-id="8331e-110">方法</span><span class="sxs-lookup"><span data-stu-id="8331e-110">Methods</span></span>
|<span data-ttu-id="8331e-111">方法</span><span class="sxs-lookup"><span data-stu-id="8331e-111">Method</span></span>|<span data-ttu-id="8331e-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="8331e-112">Return Type</span></span>|<span data-ttu-id="8331e-113">说明</span><span class="sxs-lookup"><span data-stu-id="8331e-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8331e-114">获取 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="8331e-114">Get deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-get.md)|[<span data-ttu-id="8331e-115">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="8331e-115">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="8331e-116">读取[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8331e-116">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="8331e-117">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="8331e-117">Update deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-update.md)|[<span data-ttu-id="8331e-118">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="8331e-118">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="8331e-119">更新[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8331e-119">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|<span data-ttu-id="8331e-120">**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="8331e-120">**Resource Access Policy**</span></span>|
|[<span data-ttu-id="8331e-121">列出 deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="8331e-121">List deviceManagementDerivedCredentialSettingses</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-list.md)|<span data-ttu-id="8331e-122">[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)集合</span><span class="sxs-lookup"><span data-stu-id="8331e-122">[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) collection</span></span>|<span data-ttu-id="8331e-123">列出[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8331e-123">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>|
[<span data-ttu-id="8331e-124">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="8331e-124">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="8331e-125">创建新的[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8331e-125">Create a new [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="8331e-126">删除 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="8331e-126">Delete deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-delete.md)|<span data-ttu-id="8331e-127">无</span><span class="sxs-lookup"><span data-stu-id="8331e-127">None</span></span>|<span data-ttu-id="8331e-128">删除[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="8331e-128">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>|


## <a name="properties"></a><span data-ttu-id="8331e-129">属性</span><span class="sxs-lookup"><span data-stu-id="8331e-129">Properties</span></span>
|<span data-ttu-id="8331e-130">属性</span><span class="sxs-lookup"><span data-stu-id="8331e-130">Property</span></span>|<span data-ttu-id="8331e-131">类型</span><span class="sxs-lookup"><span data-stu-id="8331e-131">Type</span></span>|<span data-ttu-id="8331e-132">说明</span><span class="sxs-lookup"><span data-stu-id="8331e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8331e-133">id</span><span class="sxs-lookup"><span data-stu-id="8331e-133">id</span></span>|<span data-ttu-id="8331e-134">String</span><span class="sxs-lookup"><span data-stu-id="8331e-134">String</span></span>|<span data-ttu-id="8331e-135">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="8331e-135">Unique identifier for the Derived Credential</span></span>|

## <a name="relationships"></a><span data-ttu-id="8331e-136">关系</span><span class="sxs-lookup"><span data-stu-id="8331e-136">Relationships</span></span>
<span data-ttu-id="8331e-137">无</span><span class="sxs-lookup"><span data-stu-id="8331e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8331e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8331e-138">JSON Representation</span></span>
<span data-ttu-id="8331e-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8331e-139">Here is a JSON representation of the resource.</span></span>
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



