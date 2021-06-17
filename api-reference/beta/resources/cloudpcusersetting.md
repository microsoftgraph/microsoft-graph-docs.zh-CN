---
title: cloudPcUserSetting 资源类型
description: 表示云电脑用户设置
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 324d2ba65c82b44595fff366c5d6eb25005c20ef
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993684"
---
# <a name="cloudpcusersetting-resource-type"></a><span data-ttu-id="e2789-103">cloudPcUserSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2789-103">cloudPcUserSetting resource type</span></span>

<span data-ttu-id="e2789-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2789-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2789-105">表示云电脑用户设置。</span><span class="sxs-lookup"><span data-stu-id="e2789-105">Represents a cloud PC user setting.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="e2789-106">方法</span><span class="sxs-lookup"><span data-stu-id="e2789-106">Methods</span></span>
|<span data-ttu-id="e2789-107">方法</span><span class="sxs-lookup"><span data-stu-id="e2789-107">Method</span></span>|<span data-ttu-id="e2789-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2789-108">Return type</span></span>|<span data-ttu-id="e2789-109">说明</span><span class="sxs-lookup"><span data-stu-id="e2789-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2789-110">列出 cloudPcUserSettings</span><span class="sxs-lookup"><span data-stu-id="e2789-110">List cloudPcUserSettings</span></span>](../api/virtualendpoint-list-usersettings.md)|<span data-ttu-id="e2789-111">[cloudPcUserSetting](../resources/cloudpcusersetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2789-111">[cloudPcUserSetting](../resources/cloudpcusersetting.md) collection</span></span>|<span data-ttu-id="e2789-112">获取 [cloudPcUserSetting 对象](../resources/cloudpcusersetting.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="e2789-112">Get a list of the [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects and their properties.</span></span>|
|[<span data-ttu-id="e2789-113">获取 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="e2789-113">Get cloudPcUserSetting</span></span>](../api/cloudpcusersetting-get.md)|[<span data-ttu-id="e2789-114">cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="e2789-114">cloudPcUserSetting</span></span>](../resources/cloudpcusersetting.md)|<span data-ttu-id="e2789-115">读取 [cloudPcUserSetting 对象的属性和](../resources/cloudpcusersetting.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="e2789-115">Read the properties and relationships of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>|
|[<span data-ttu-id="e2789-116">创建 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="e2789-116">Create cloudPcUserSetting</span></span>](../api/virtualendpoint-post-usersettings.md)|[<span data-ttu-id="e2789-117">cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="e2789-117">cloudPcUserSetting</span></span>](../resources/cloudpcusersetting.md)|<span data-ttu-id="e2789-118">创建新的 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2789-118">Create a new [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>|
|[<span data-ttu-id="e2789-119">更新 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="e2789-119">Update cloudPcUserSetting</span></span>](../api/cloudpcusersetting-update.md)|[<span data-ttu-id="e2789-120">cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="e2789-120">cloudPcUserSetting</span></span>](../resources/cloudpcusersetting.md)|<span data-ttu-id="e2789-121">更新 [cloudPcUserSetting 对象](../resources/cloudpcusersetting.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="e2789-121">Update the properties of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>|
|[<span data-ttu-id="e2789-122">删除 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="e2789-122">Delete cloudPcUserSetting</span></span>](../api/cloudpcusersetting-delete.md)|<span data-ttu-id="e2789-123">无</span><span class="sxs-lookup"><span data-stu-id="e2789-123">None</span></span>|<span data-ttu-id="e2789-124">删除 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2789-124">Deletes a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>|
|[<span data-ttu-id="e2789-125">assign</span><span class="sxs-lookup"><span data-stu-id="e2789-125">assign</span></span>](../api/cloudpcusersetting-assign.md)|<span data-ttu-id="e2789-126">无</span><span class="sxs-lookup"><span data-stu-id="e2789-126">None</span></span>|<span data-ttu-id="e2789-127">将 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 分配给用户组。</span><span class="sxs-lookup"><span data-stu-id="e2789-127">Assign a [cloudPcUserSetting](../resources/cloudpcusersetting.md) to user groups.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2789-128">属性</span><span class="sxs-lookup"><span data-stu-id="e2789-128">Properties</span></span>
|<span data-ttu-id="e2789-129">属性</span><span class="sxs-lookup"><span data-stu-id="e2789-129">Property</span></span>|<span data-ttu-id="e2789-130">类型</span><span class="sxs-lookup"><span data-stu-id="e2789-130">Type</span></span>|<span data-ttu-id="e2789-131">说明</span><span class="sxs-lookup"><span data-stu-id="e2789-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2789-132">id</span><span class="sxs-lookup"><span data-stu-id="e2789-132">id</span></span>|<span data-ttu-id="e2789-133">String</span><span class="sxs-lookup"><span data-stu-id="e2789-133">String</span></span>|<span data-ttu-id="e2789-134">云电脑用户设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e2789-134">Unique identifier for the cloud PC user setting.</span></span> <span data-ttu-id="e2789-135">只读。</span><span class="sxs-lookup"><span data-stu-id="e2789-135">Read-only.</span></span>|
|<span data-ttu-id="e2789-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e2789-136">displayName</span></span>|<span data-ttu-id="e2789-137">String</span><span class="sxs-lookup"><span data-stu-id="e2789-137">String</span></span>|<span data-ttu-id="e2789-138">用户界面中显示的设置名称。</span><span class="sxs-lookup"><span data-stu-id="e2789-138">The setting name displayed in the user interface.</span></span> |
|<span data-ttu-id="e2789-139">localAdminEnabled</span><span class="sxs-lookup"><span data-stu-id="e2789-139">localAdminEnabled</span></span>|<span data-ttu-id="e2789-140">布尔</span><span class="sxs-lookup"><span data-stu-id="e2789-140">Boolean</span></span>|<span data-ttu-id="e2789-141">指示是否已启用本地管理员选项。</span><span class="sxs-lookup"><span data-stu-id="e2789-141">Indicates whether the local admin option is enabled.</span></span> <span data-ttu-id="e2789-142">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e2789-142">Default value is `false`.</span></span> <span data-ttu-id="e2789-143">若要启用本地管理员选项，将设置更改为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="e2789-143">To enable the local admin option, change the setting to `true`.</span></span> |
|<span data-ttu-id="e2789-144">selfServiceEnabled</span><span class="sxs-lookup"><span data-stu-id="e2789-144">selfServiceEnabled</span></span>|<span data-ttu-id="e2789-145">布尔</span><span class="sxs-lookup"><span data-stu-id="e2789-145">Boolean</span></span>|<span data-ttu-id="e2789-146">指示是否已启用自助服务选项。</span><span class="sxs-lookup"><span data-stu-id="e2789-146">Indicates whether the self-service option is enabled.</span></span> <span data-ttu-id="e2789-147">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="e2789-147">Default value is `false`.</span></span> <span data-ttu-id="e2789-148">若要启用自助服务选项，将设置更改为 `true` 。 </span><span class="sxs-lookup"><span data-stu-id="e2789-148">To enable the self-service option, change the setting to `true`. </span></span>|
|<span data-ttu-id="e2789-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2789-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e2789-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2789-150">DateTimeOffset</span></span>|<span data-ttu-id="e2789-151">上次修改设置的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2789-151">The last date and time the setting was modified.</span></span> <span data-ttu-id="e2789-152">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e2789-152">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e2789-153">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="e2789-153">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |
|<span data-ttu-id="e2789-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2789-154">createdDateTime</span></span>|<span data-ttu-id="e2789-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2789-155">DateTimeOffset</span></span>|<span data-ttu-id="e2789-156">创建设置的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2789-156">The date and time the setting was created.</span></span> <span data-ttu-id="e2789-157">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e2789-157">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e2789-158">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="e2789-158">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e2789-159">关系</span><span class="sxs-lookup"><span data-stu-id="e2789-159">Relationships</span></span>
|<span data-ttu-id="e2789-160">关系</span><span class="sxs-lookup"><span data-stu-id="e2789-160">Relationship</span></span>|<span data-ttu-id="e2789-161">类型</span><span class="sxs-lookup"><span data-stu-id="e2789-161">Type</span></span>|<span data-ttu-id="e2789-162">说明</span><span class="sxs-lookup"><span data-stu-id="e2789-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2789-163">assignments</span><span class="sxs-lookup"><span data-stu-id="e2789-163">assignments</span></span>|<span data-ttu-id="e2789-164">[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2789-164">[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) collection</span></span>|<span data-ttu-id="e2789-165">Office 365 Azure AD 中的安全组可以分配一组用户设置。</span><span class="sxs-lookup"><span data-stu-id="e2789-165">Office 365 and security groups in Azure AD can have a set of user settings assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2789-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2789-166">JSON representation</span></span>
<span data-ttu-id="e2789-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2789-167">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSetting",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "id": "String (identifier)",
  "displayName": "String",
  "selfServiceEnabled": "Boolean",
  "localAdminEnabled": "Boolean",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```
