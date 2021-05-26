---
title: chromeOSOnboardingSettings 资源类型
description: 表示 Chromebook 租户设置的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 442ea58414febe146745892844f8667c8fd799a3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666990"
---
# <a name="chromeosonboardingsettings-resource-type"></a><span data-ttu-id="b9ecf-103">chromeOSOnboardingSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9ecf-103">chromeOSOnboardingSettings resource type</span></span>

<span data-ttu-id="b9ecf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9ecf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9ecf-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9ecf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9ecf-107">表示 Chromebook 租户设置的实体</span><span class="sxs-lookup"><span data-stu-id="b9ecf-107">Entity that represents a Chromebook tenant settings</span></span>

## <a name="methods"></a><span data-ttu-id="b9ecf-108">方法</span><span class="sxs-lookup"><span data-stu-id="b9ecf-108">Methods</span></span>
|<span data-ttu-id="b9ecf-109">方法</span><span class="sxs-lookup"><span data-stu-id="b9ecf-109">Method</span></span>|<span data-ttu-id="b9ecf-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b9ecf-110">Return Type</span></span>|<span data-ttu-id="b9ecf-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9ecf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b9ecf-112">列出 chromeOSOnboardingSettingses</span><span class="sxs-lookup"><span data-stu-id="b9ecf-112">List chromeOSOnboardingSettingses</span></span>](../api/intune-chromebooksync-chromeosonboardingsettings-list.md)|<span data-ttu-id="b9ecf-113">[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b9ecf-113">[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) collection</span></span>|<span data-ttu-id="b9ecf-114">列出 [chromeOSOnboardingSettings 对象的属性和](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-114">List properties and relationships of the [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) objects.</span></span>|
|[<span data-ttu-id="b9ecf-115">获取 chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="b9ecf-115">Get chromeOSOnboardingSettings</span></span>](../api/intune-chromebooksync-chromeosonboardingsettings-get.md)|[<span data-ttu-id="b9ecf-116">chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="b9ecf-116">chromeOSOnboardingSettings</span></span>](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|<span data-ttu-id="b9ecf-117">读取 [chromeOSOnboardingSettings 对象的属性和](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-117">Read properties and relationships of the [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>|
|[<span data-ttu-id="b9ecf-118">创建 chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="b9ecf-118">Create chromeOSOnboardingSettings</span></span>](../api/intune-chromebooksync-chromeosonboardingsettings-create.md)|[<span data-ttu-id="b9ecf-119">chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="b9ecf-119">chromeOSOnboardingSettings</span></span>](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|<span data-ttu-id="b9ecf-120">创建新的 [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-120">Create a new [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>|
|[<span data-ttu-id="b9ecf-121">删除 chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="b9ecf-121">Delete chromeOSOnboardingSettings</span></span>](../api/intune-chromebooksync-chromeosonboardingsettings-delete.md)|<span data-ttu-id="b9ecf-122">无</span><span class="sxs-lookup"><span data-stu-id="b9ecf-122">None</span></span>|<span data-ttu-id="b9ecf-123">删除 [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-123">Deletes a [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md).</span></span>|
|[<span data-ttu-id="b9ecf-124">更新 chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="b9ecf-124">Update chromeOSOnboardingSettings</span></span>](../api/intune-chromebooksync-chromeosonboardingsettings-update.md)|[<span data-ttu-id="b9ecf-125">chromeOSOnboardingSettings</span><span class="sxs-lookup"><span data-stu-id="b9ecf-125">chromeOSOnboardingSettings</span></span>](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|<span data-ttu-id="b9ecf-126">更新 [chromeOSOnboardingSettings 对象](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-126">Update the properties of a [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) object.</span></span>|
|[<span data-ttu-id="b9ecf-127">connect 操作</span><span class="sxs-lookup"><span data-stu-id="b9ecf-127">connect action</span></span>](../api/intune-chromebooksync-chromeosonboardingsettings-connect.md)|[<span data-ttu-id="b9ecf-128">chromeOSOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="b9ecf-128">chromeOSOnboardingStatus</span></span>](../resources/intune-chromebooksync-chromeosonboardingstatus.md)|<span data-ttu-id="b9ecf-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b9ecf-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b9ecf-130">属性</span><span class="sxs-lookup"><span data-stu-id="b9ecf-130">Properties</span></span>
|<span data-ttu-id="b9ecf-131">属性</span><span class="sxs-lookup"><span data-stu-id="b9ecf-131">Property</span></span>|<span data-ttu-id="b9ecf-132">类型</span><span class="sxs-lookup"><span data-stu-id="b9ecf-132">Type</span></span>|<span data-ttu-id="b9ecf-133">说明</span><span class="sxs-lookup"><span data-stu-id="b9ecf-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9ecf-134">id</span><span class="sxs-lookup"><span data-stu-id="b9ecf-134">id</span></span>|<span data-ttu-id="b9ecf-135">String</span><span class="sxs-lookup"><span data-stu-id="b9ecf-135">String</span></span>|<span data-ttu-id="b9ecf-136">ChromebookTenant 的 ID</span><span class="sxs-lookup"><span data-stu-id="b9ecf-136">The ChromebookTenant's Id</span></span>|
|<span data-ttu-id="b9ecf-137">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9ecf-137">ownerUserPrincipalName</span></span>|<span data-ttu-id="b9ecf-138">String</span><span class="sxs-lookup"><span data-stu-id="b9ecf-138">String</span></span>|<span data-ttu-id="b9ecf-139">ChromebookTenant 的 OwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9ecf-139">The ChromebookTenant's OwnerUserPrincipalName</span></span>|
|<span data-ttu-id="b9ecf-140">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="b9ecf-140">onboardingStatus</span></span>|[<span data-ttu-id="b9ecf-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="b9ecf-141">onboardingStatus</span></span>](../resources/intune-chromebooksync-onboardingstatus.md)|<span data-ttu-id="b9ecf-142">ChromebookTenant 的 OnboardingStatus。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-142">The ChromebookTenant's OnboardingStatus.</span></span> <span data-ttu-id="b9ecf-143">可取值为：`unknown`、`inprogress`、`onboarded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-143">Possible values are: `unknown`, `inprogress`, `onboarded`, `failed`.</span></span>|
|<span data-ttu-id="b9ecf-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9ecf-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b9ecf-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9ecf-145">DateTimeOffset</span></span>|<span data-ttu-id="b9ecf-146">ChromebookTenant 的 LastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9ecf-146">The ChromebookTenant's LastModifiedDateTime</span></span>|
|<span data-ttu-id="b9ecf-147">lastDirectorySyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b9ecf-147">lastDirectorySyncDateTime</span></span>|<span data-ttu-id="b9ecf-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9ecf-148">DateTimeOffset</span></span>|<span data-ttu-id="b9ecf-149">ChromebookTenant 的 LastDirectorySyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b9ecf-149">The ChromebookTenant's LastDirectorySyncDateTime</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9ecf-150">关系</span><span class="sxs-lookup"><span data-stu-id="b9ecf-150">Relationships</span></span>
<span data-ttu-id="b9ecf-151">无</span><span class="sxs-lookup"><span data-stu-id="b9ecf-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9ecf-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9ecf-152">JSON Representation</span></span>
<span data-ttu-id="b9ecf-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9ecf-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chromeOSOnboardingSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "id": "String (identifier)",
  "ownerUserPrincipalName": "String",
  "onboardingStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastDirectorySyncDateTime": "String (timestamp)"
}
```




