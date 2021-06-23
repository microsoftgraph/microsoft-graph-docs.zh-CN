---
title: cloudPcUserSetting 资源类型
description: 表示云电脑用户设置
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 534e2b14e7df4f8b571e14e1238ad6ed03d96a67
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082158"
---
# <a name="cloudpcusersetting-resource-type"></a><span data-ttu-id="66de1-103">cloudPcUserSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="66de1-103">cloudPcUserSetting resource type</span></span>

<span data-ttu-id="66de1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66de1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66de1-105">表示云电脑用户设置。</span><span class="sxs-lookup"><span data-stu-id="66de1-105">Represents a cloud PC user setting.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="66de1-106">方法</span><span class="sxs-lookup"><span data-stu-id="66de1-106">Methods</span></span>
|<span data-ttu-id="66de1-107">方法</span><span class="sxs-lookup"><span data-stu-id="66de1-107">Method</span></span>|<span data-ttu-id="66de1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="66de1-108">Return type</span></span>|<span data-ttu-id="66de1-109">说明</span><span class="sxs-lookup"><span data-stu-id="66de1-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66de1-110">列出 cloudPcUserSettings</span><span class="sxs-lookup"><span data-stu-id="66de1-110">List cloudPcUserSettings</span></span>](../api/virtualendpoint-list-usersettings.md)|<span data-ttu-id="66de1-111">[cloudPcUserSetting](../resources/cloudpcusersetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66de1-111">[cloudPcUserSetting](../resources/cloudpcusersetting.md) collection</span></span>|<span data-ttu-id="66de1-112">获取 [cloudPcUserSetting 对象](../resources/cloudpcusersetting.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="66de1-112">Get a list of the [cloudPcUserSetting](../resources/cloudpcusersetting.md) objects and their properties.</span></span>|
|[<span data-ttu-id="66de1-113">获取 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="66de1-113">Get cloudPcUserSetting</span></span>](../api/cloudpcusersetting-get.md)|[<span data-ttu-id="66de1-114">cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="66de1-114">cloudPcUserSetting</span></span>](../resources/cloudpcusersetting.md)|<span data-ttu-id="66de1-115">读取 [cloudPcUserSetting 对象的属性和](../resources/cloudpcusersetting.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="66de1-115">Read the properties and relationships of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>|
|[<span data-ttu-id="66de1-116">创建 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="66de1-116">Create cloudPcUserSetting</span></span>](../api/virtualendpoint-post-usersettings.md)|[<span data-ttu-id="66de1-117">cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="66de1-117">cloudPcUserSetting</span></span>](../resources/cloudpcusersetting.md)|<span data-ttu-id="66de1-118">创建新的 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66de1-118">Create a new [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>|
|[<span data-ttu-id="66de1-119">更新 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="66de1-119">Update cloudPcUserSetting</span></span>](../api/cloudpcusersetting-update.md)|[<span data-ttu-id="66de1-120">cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="66de1-120">cloudPcUserSetting</span></span>](../resources/cloudpcusersetting.md)|<span data-ttu-id="66de1-121">更新 [cloudPcUserSetting 对象](../resources/cloudpcusersetting.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="66de1-121">Update the properties of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>|
|[<span data-ttu-id="66de1-122">删除 cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="66de1-122">Delete cloudPcUserSetting</span></span>](../api/cloudpcusersetting-delete.md)|<span data-ttu-id="66de1-123">无</span><span class="sxs-lookup"><span data-stu-id="66de1-123">None</span></span>|<span data-ttu-id="66de1-124">删除 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66de1-124">Deletes a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>|
|[<span data-ttu-id="66de1-125">Assign</span><span class="sxs-lookup"><span data-stu-id="66de1-125">Assign</span></span>](../api/cloudpcusersetting-assign.md)|<span data-ttu-id="66de1-126">无</span><span class="sxs-lookup"><span data-stu-id="66de1-126">None</span></span>|<span data-ttu-id="66de1-127">将 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 分配给用户组。</span><span class="sxs-lookup"><span data-stu-id="66de1-127">Assign a [cloudPcUserSetting](../resources/cloudpcusersetting.md) to user groups.</span></span>|

## <a name="properties"></a><span data-ttu-id="66de1-128">属性</span><span class="sxs-lookup"><span data-stu-id="66de1-128">Properties</span></span>
|<span data-ttu-id="66de1-129">属性</span><span class="sxs-lookup"><span data-stu-id="66de1-129">Property</span></span>|<span data-ttu-id="66de1-130">类型</span><span class="sxs-lookup"><span data-stu-id="66de1-130">Type</span></span>|<span data-ttu-id="66de1-131">说明</span><span class="sxs-lookup"><span data-stu-id="66de1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66de1-132">id</span><span class="sxs-lookup"><span data-stu-id="66de1-132">id</span></span>|<span data-ttu-id="66de1-133">String</span><span class="sxs-lookup"><span data-stu-id="66de1-133">String</span></span>|<span data-ttu-id="66de1-134">云电脑用户设置的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="66de1-134">Unique identifier for the cloud PC user setting.</span></span> <span data-ttu-id="66de1-135">只读。</span><span class="sxs-lookup"><span data-stu-id="66de1-135">Read-only.</span></span>|
|<span data-ttu-id="66de1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="66de1-136">displayName</span></span>|<span data-ttu-id="66de1-137">String</span><span class="sxs-lookup"><span data-stu-id="66de1-137">String</span></span>|<span data-ttu-id="66de1-138">用户界面中显示的设置名称。</span><span class="sxs-lookup"><span data-stu-id="66de1-138">The setting name displayed in the user interface.</span></span> |
|<span data-ttu-id="66de1-139">localAdminEnabled</span><span class="sxs-lookup"><span data-stu-id="66de1-139">localAdminEnabled</span></span>|<span data-ttu-id="66de1-140">布尔值</span><span class="sxs-lookup"><span data-stu-id="66de1-140">Boolean</span></span>|<span data-ttu-id="66de1-141">指示是否已启用本地管理员选项。</span><span class="sxs-lookup"><span data-stu-id="66de1-141">Indicates whether the local admin option is enabled.</span></span> <span data-ttu-id="66de1-142">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="66de1-142">Default value is `false`.</span></span> <span data-ttu-id="66de1-143">若要启用本地管理员选项，将设置更改为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="66de1-143">To enable the local admin option, change the setting to `true`.</span></span> <span data-ttu-id="66de1-144">如果启用了本地管理员选项，最终用户可以是云电脑设备的管理员。</span><span class="sxs-lookup"><span data-stu-id="66de1-144">If the local admin option is enabled, the end user can be an admin of the cloud PC device.</span></span> |
|<span data-ttu-id="66de1-145">selfServiceEnabled</span><span class="sxs-lookup"><span data-stu-id="66de1-145">selfServiceEnabled</span></span>|<span data-ttu-id="66de1-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="66de1-146">Boolean</span></span>|<span data-ttu-id="66de1-147">指示是否已启用自助服务选项。</span><span class="sxs-lookup"><span data-stu-id="66de1-147">Indicates whether the self-service option is enabled.</span></span> <span data-ttu-id="66de1-148">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="66de1-148">Default value is `false`.</span></span> <span data-ttu-id="66de1-149">若要启用自助服务选项，将设置更改为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="66de1-149">To enable the self-service option, change the setting to `true`.</span></span><span data-ttu-id="66de1-150">如果启用自助服务选项，则允许最终用户执行一些自助服务操作，例如通过最终用户门户升级云电脑。</span><span class="sxs-lookup"><span data-stu-id="66de1-150"> If the self-service option is enabled, the end user is allowed to perform some self-service operations, such as upgrading the cloud PC through the end user portal.</span></span>|
|<span data-ttu-id="66de1-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66de1-151">lastModifiedDateTime</span></span>|<span data-ttu-id="66de1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66de1-152">DateTimeOffset</span></span>|<span data-ttu-id="66de1-153">上次修改设置的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="66de1-153">The last date and time the setting was modified.</span></span> <span data-ttu-id="66de1-154">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="66de1-154">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66de1-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="66de1-155">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |
|<span data-ttu-id="66de1-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66de1-156">createdDateTime</span></span>|<span data-ttu-id="66de1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66de1-157">DateTimeOffset</span></span>|<span data-ttu-id="66de1-158">创建设置的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="66de1-158">The date and time the setting was created.</span></span> <span data-ttu-id="66de1-159">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="66de1-159">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66de1-160">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="66de1-160">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span> |

## <a name="relationships"></a><span data-ttu-id="66de1-161">关系</span><span class="sxs-lookup"><span data-stu-id="66de1-161">Relationships</span></span>
|<span data-ttu-id="66de1-162">关系</span><span class="sxs-lookup"><span data-stu-id="66de1-162">Relationship</span></span>|<span data-ttu-id="66de1-163">类型</span><span class="sxs-lookup"><span data-stu-id="66de1-163">Type</span></span>|<span data-ttu-id="66de1-164">说明</span><span class="sxs-lookup"><span data-stu-id="66de1-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66de1-165">assignments</span><span class="sxs-lookup"><span data-stu-id="66de1-165">assignments</span></span>|<span data-ttu-id="66de1-166">[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="66de1-166">[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) collection</span></span>|<span data-ttu-id="66de1-167">表示已Microsoft 365 cloudPCUserSetting 的 Azure AD 中的组和安全组集。</span><span class="sxs-lookup"><span data-stu-id="66de1-167">Represents the set of Microsoft 365 groups and security groups in Azure AD that have cloudPCUserSetting assigned.</span></span> <span data-ttu-id="66de1-168">仅在 `$expand` 上返回。</span><span class="sxs-lookup"><span data-stu-id="66de1-168">Returned only on `$expand`.</span></span> <span data-ttu-id="66de1-169">有关示例，请参阅 [获取 cloudPcUserSettingample](../api/cloudpcusersetting-get.md)。</span><span class="sxs-lookup"><span data-stu-id="66de1-169">For an example, see [Get cloudPcUserSettingample](../api/cloudpcusersetting-get.md).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66de1-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66de1-170">JSON representation</span></span>
<span data-ttu-id="66de1-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66de1-171">The following is a JSON representation of the resource.</span></span>
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
