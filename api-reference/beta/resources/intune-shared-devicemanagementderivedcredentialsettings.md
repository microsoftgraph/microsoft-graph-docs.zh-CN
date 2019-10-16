---
title: deviceManagementDerivedCredentialSettings 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f7bf6bdf486e73d72ad227596b9ab1e7dcbe0386
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538740"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a><span data-ttu-id="60465-103">deviceManagementDerivedCredentialSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="60465-103">deviceManagementDerivedCredentialSettings resource type</span></span>

> <span data-ttu-id="60465-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="60465-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60465-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60465-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60465-106">DeviceManagementDerivedCredentialSettings 资源代表其内容因工作流而异的容器，包括：</span><span class="sxs-lookup"><span data-stu-id="60465-106">The deviceManagementDerivedCredentialSettings resource represents a container whose contents vary according to workflow, including:</span></span>  

- <span data-ttu-id="60465-107">设备配置设置</span><span class="sxs-lookup"><span data-stu-id="60465-107">Device configuration settings</span></span>
- <span data-ttu-id="60465-108">RA 策略</span><span class="sxs-lookup"><span data-stu-id="60465-108">RA Policy</span></span>

## <a name="methods"></a><span data-ttu-id="60465-109">方法</span><span class="sxs-lookup"><span data-stu-id="60465-109">Methods</span></span>
|<span data-ttu-id="60465-110">方法</span><span class="sxs-lookup"><span data-stu-id="60465-110">Method</span></span>|<span data-ttu-id="60465-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="60465-111">Return Type</span></span>|<span data-ttu-id="60465-112">说明</span><span class="sxs-lookup"><span data-stu-id="60465-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60465-113">获取 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="60465-113">Get deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-get.md)|[<span data-ttu-id="60465-114">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="60465-114">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="60465-115">读取[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="60465-115">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="60465-116">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="60465-116">Update deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-update.md)|[<span data-ttu-id="60465-117">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="60465-117">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="60465-118">更新[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="60465-118">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|<span data-ttu-id="60465-119">**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="60465-119">**Resource Access Policy**</span></span>|
|[<span data-ttu-id="60465-120">列出 deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="60465-120">List deviceManagementDerivedCredentialSettingses</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-list.md)|<span data-ttu-id="60465-121">[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)集合</span><span class="sxs-lookup"><span data-stu-id="60465-121">[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) collection</span></span>|<span data-ttu-id="60465-122">列出[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="60465-122">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>|
[<span data-ttu-id="60465-123">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="60465-123">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="60465-124">创建新的[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="60465-124">Create a new [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="60465-125">删除 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="60465-125">Delete deviceManagementDerivedCredentialSettings</span></span>](../api/intune-shared-devicemanagementderivedcredentialsettings-delete.md)|<span data-ttu-id="60465-126">无</span><span class="sxs-lookup"><span data-stu-id="60465-126">None</span></span>|<span data-ttu-id="60465-127">删除[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="60465-127">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>|


## <a name="properties"></a><span data-ttu-id="60465-128">属性</span><span class="sxs-lookup"><span data-stu-id="60465-128">Properties</span></span>
|<span data-ttu-id="60465-129">属性</span><span class="sxs-lookup"><span data-stu-id="60465-129">Property</span></span>|<span data-ttu-id="60465-130">类型</span><span class="sxs-lookup"><span data-stu-id="60465-130">Type</span></span>|<span data-ttu-id="60465-131">说明</span><span class="sxs-lookup"><span data-stu-id="60465-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60465-132">id</span><span class="sxs-lookup"><span data-stu-id="60465-132">id</span></span>|<span data-ttu-id="60465-133">字符串</span><span class="sxs-lookup"><span data-stu-id="60465-133">String</span></span>|<span data-ttu-id="60465-134">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="60465-134">Unique identifier for the Derived Credential</span></span>|

## <a name="relationships"></a><span data-ttu-id="60465-135">关系</span><span class="sxs-lookup"><span data-stu-id="60465-135">Relationships</span></span>
<span data-ttu-id="60465-136">无</span><span class="sxs-lookup"><span data-stu-id="60465-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60465-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60465-137">JSON Representation</span></span>
<span data-ttu-id="60465-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60465-138">Here is a JSON representation of the resource.</span></span>
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



