---
title: deviceManagementDerivedCredentialSettings 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5b3b33049d01d14c5c0800910138ceef1245d29
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730381"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a><span data-ttu-id="c3d4d-103">deviceManagementDerivedCredentialSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3d4d-103">deviceManagementDerivedCredentialSettings resource type</span></span>

<span data-ttu-id="c3d4d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3d4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3d4d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3d4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3d4d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3d4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3d4d-107">DeviceManagementDerivedCredentialSettings 资源代表其内容因工作流而异的容器，包括：</span><span class="sxs-lookup"><span data-stu-id="c3d4d-107">The deviceManagementDerivedCredentialSettings resource represents a container whose contents vary according to workflow, including:</span></span>

- <span data-ttu-id="c3d4d-108">设备配置设置</span><span class="sxs-lookup"><span data-stu-id="c3d4d-108">Device configuration settings</span></span>
- <span data-ttu-id="c3d4d-109">RA 策略</span><span class="sxs-lookup"><span data-stu-id="c3d4d-109">RA Policy</span></span>

## <a name="methods"></a><span data-ttu-id="c3d4d-110">Methods</span><span class="sxs-lookup"><span data-stu-id="c3d4d-110">Methods</span></span>
|<span data-ttu-id="c3d4d-111">方法</span><span class="sxs-lookup"><span data-stu-id="c3d4d-111">Method</span></span>|<span data-ttu-id="c3d4d-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c3d4d-112">Return Type</span></span>|<span data-ttu-id="c3d4d-113">说明</span><span class="sxs-lookup"><span data-stu-id="c3d4d-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3d4d-114">获取 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="c3d4d-114">Get deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-get.md)|[<span data-ttu-id="c3d4d-115">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="c3d4d-115">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="c3d4d-116">读取 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c3d4d-116">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="c3d4d-117">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="c3d4d-117">Update deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-update.md)|[<span data-ttu-id="c3d4d-118">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="c3d4d-118">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="c3d4d-119">更新 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3d4d-119">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|<span data-ttu-id="c3d4d-120">**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="c3d4d-120">**Resource Access Policy**</span></span>|
|[<span data-ttu-id="c3d4d-121">列出 deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="c3d4d-121">List deviceManagementDerivedCredentialSettingses</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-list.md)|<span data-ttu-id="c3d4d-122">[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c3d4d-122">[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) collection</span></span>|<span data-ttu-id="c3d4d-123">列出 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c3d4d-123">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>|
[<span data-ttu-id="c3d4d-124">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="c3d4d-124">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="c3d4d-125">创建新的 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3d4d-125">Create a new [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="c3d4d-126">删除 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="c3d4d-126">Delete deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-delete.md)|<span data-ttu-id="c3d4d-127">无</span><span class="sxs-lookup"><span data-stu-id="c3d4d-127">None</span></span>|<span data-ttu-id="c3d4d-128">删除 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="c3d4d-128">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>|


## <a name="properties"></a><span data-ttu-id="c3d4d-129">属性</span><span class="sxs-lookup"><span data-stu-id="c3d4d-129">Properties</span></span>
|<span data-ttu-id="c3d4d-130">属性</span><span class="sxs-lookup"><span data-stu-id="c3d4d-130">Property</span></span>|<span data-ttu-id="c3d4d-131">类型</span><span class="sxs-lookup"><span data-stu-id="c3d4d-131">Type</span></span>|<span data-ttu-id="c3d4d-132">说明</span><span class="sxs-lookup"><span data-stu-id="c3d4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3d4d-133">id</span><span class="sxs-lookup"><span data-stu-id="c3d4d-133">id</span></span>|<span data-ttu-id="c3d4d-134">String</span><span class="sxs-lookup"><span data-stu-id="c3d4d-134">String</span></span>|<span data-ttu-id="c3d4d-135">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="c3d4d-135">Unique identifier for the Derived Credential</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3d4d-136">关系</span><span class="sxs-lookup"><span data-stu-id="c3d4d-136">Relationships</span></span>
<span data-ttu-id="c3d4d-137">无</span><span class="sxs-lookup"><span data-stu-id="c3d4d-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3d4d-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3d4d-138">JSON Representation</span></span>
<span data-ttu-id="c3d4d-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3d4d-139">Here is a JSON representation of the resource.</span></span>
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





