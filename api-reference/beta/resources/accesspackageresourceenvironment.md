---
title: accessPackageResourceEnvironment 资源类型
description: 访问包资源环境是资源所在的地理位置环境的引用。
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b21c0f1ae8fd70ac2df76dfa50bc886bca04de19
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760853"
---
# <a name="accesspackageresourceenvironment-resource-type"></a><span data-ttu-id="22bd8-103">accessPackageResourceEnvironment 资源类型</span><span class="sxs-lookup"><span data-stu-id="22bd8-103">accessPackageResourceEnvironment resource type</span></span>

<span data-ttu-id="22bd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22bd8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22bd8-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源环境是资源所在的地理位置环境的引用。</span><span class="sxs-lookup"><span data-stu-id="22bd8-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource environment is a reference to the geolocation environment in which a resource is located.</span></span> <span data-ttu-id="22bd8-106">此环境自动作为 Azure AD 权利管理的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="22bd8-106">This environment is automatically provided as part of Azure AD Entitlement Management.</span></span> <span data-ttu-id="22bd8-107">此 API 仅适用于多地理位置 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="22bd8-107">The API is only applicable to Multi-Geo SharePoint Online sites.</span></span>

## <a name="methods"></a><span data-ttu-id="22bd8-108">方法</span><span class="sxs-lookup"><span data-stu-id="22bd8-108">Methods</span></span>
|<span data-ttu-id="22bd8-109">方法</span><span class="sxs-lookup"><span data-stu-id="22bd8-109">Method</span></span>|<span data-ttu-id="22bd8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="22bd8-110">Return type</span></span>|<span data-ttu-id="22bd8-111">说明</span><span class="sxs-lookup"><span data-stu-id="22bd8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="22bd8-112">列出 accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="22bd8-112">List accessPackageResourceEnvironments</span></span>](../api/accesspackageresourceenvironment-list.md)|<span data-ttu-id="22bd8-113">[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22bd8-113">[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection</span></span>|<span data-ttu-id="22bd8-114">检索 [accessPackageResourceEnvironment 对象](../resources/accesspackageresourceenvironment.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="22bd8-114">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects.</span></span>|
|[<span data-ttu-id="22bd8-115">获取 accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="22bd8-115">Get accessPackageResourceEnvironment</span></span>](../api/accesspackageresourceenvironment-get.md)|[<span data-ttu-id="22bd8-116">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="22bd8-116">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="22bd8-117">读取 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22bd8-117">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="22bd8-118">属性</span><span class="sxs-lookup"><span data-stu-id="22bd8-118">Properties</span></span>
|<span data-ttu-id="22bd8-119">属性</span><span class="sxs-lookup"><span data-stu-id="22bd8-119">Property</span></span>|<span data-ttu-id="22bd8-120">类型</span><span class="sxs-lookup"><span data-stu-id="22bd8-120">Type</span></span>|<span data-ttu-id="22bd8-121">说明</span><span class="sxs-lookup"><span data-stu-id="22bd8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22bd8-122">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="22bd8-122">connectionInfo</span></span>|[<span data-ttu-id="22bd8-123">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="22bd8-123">connectionInfo</span></span>](../resources/connectioninfo.md)|<span data-ttu-id="22bd8-124">用于连接到资源的环境的连接信息。</span><span class="sxs-lookup"><span data-stu-id="22bd8-124">Connection information of an environment used to connect to a resource.</span></span> |
|<span data-ttu-id="22bd8-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="22bd8-125">createdBy</span></span>|<span data-ttu-id="22bd8-126">String</span><span class="sxs-lookup"><span data-stu-id="22bd8-126">String</span></span>|<span data-ttu-id="22bd8-127">创建显示名称的用户的组。</span><span class="sxs-lookup"><span data-stu-id="22bd8-127">The display name of the user that created this object.</span></span>|
|<span data-ttu-id="22bd8-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22bd8-128">createdDateTime</span></span>|<span data-ttu-id="22bd8-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22bd8-129">DateTimeOffset</span></span>|<span data-ttu-id="22bd8-130">创建此对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="22bd8-130">The date and time that this object was created.</span></span> <br><span data-ttu-id="22bd8-131">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="22bd8-131">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="22bd8-132">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="22bd8-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="22bd8-133">说明</span><span class="sxs-lookup"><span data-stu-id="22bd8-133">description</span></span>|<span data-ttu-id="22bd8-134">String</span><span class="sxs-lookup"><span data-stu-id="22bd8-134">String</span></span>|<span data-ttu-id="22bd8-135">此 *accessPackageResourceEnvironment 对象的* 说明。</span><span class="sxs-lookup"><span data-stu-id="22bd8-135">The description of this *accessPackageResourceEnvironment* object.</span></span>|
|<span data-ttu-id="22bd8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="22bd8-136">displayName</span></span>|<span data-ttu-id="22bd8-137">String</span><span class="sxs-lookup"><span data-stu-id="22bd8-137">String</span></span>|<span data-ttu-id="22bd8-138">此显示名称对象的对象。</span><span class="sxs-lookup"><span data-stu-id="22bd8-138">The display name of this object.</span></span>|
|<span data-ttu-id="22bd8-139">id</span><span class="sxs-lookup"><span data-stu-id="22bd8-139">id</span></span>|<span data-ttu-id="22bd8-140">String</span><span class="sxs-lookup"><span data-stu-id="22bd8-140">String</span></span>|<span data-ttu-id="22bd8-141">系统分配的对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="22bd8-141">The system-assigned unique identifier of the object.</span></span>|
|<span data-ttu-id="22bd8-142">isDefaultEnvironment</span><span class="sxs-lookup"><span data-stu-id="22bd8-142">isDefaultEnvironment</span></span>|<span data-ttu-id="22bd8-143">布尔</span><span class="sxs-lookup"><span data-stu-id="22bd8-143">Boolean</span></span>|<span data-ttu-id="22bd8-144">确定这是否是默认环境。</span><span class="sxs-lookup"><span data-stu-id="22bd8-144">Determines whether this is default environment or not.</span></span> <span data-ttu-id="22bd8-145">它设置为 `true` 所有静态源系统，如 Azure AD 组和 Azure AD 应用程序。</span><span class="sxs-lookup"><span data-stu-id="22bd8-145">It is set to `true` for all static origin systems, such as Azure AD groups and Azure AD Applications.</span></span>|
|<span data-ttu-id="22bd8-146">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="22bd8-146">modifiedBy</span></span>|<span data-ttu-id="22bd8-147">String</span><span class="sxs-lookup"><span data-stu-id="22bd8-147">String</span></span>|<span data-ttu-id="22bd8-148">最后显示名称修改此对象的实体的子项。</span><span class="sxs-lookup"><span data-stu-id="22bd8-148">The display name of the entity that last modified this object.</span></span>|
|<span data-ttu-id="22bd8-149">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22bd8-149">modifiedDateTime</span></span>|<span data-ttu-id="22bd8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22bd8-150">DateTimeOffset</span></span>|<span data-ttu-id="22bd8-151">上次修改此对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="22bd8-151">The date and time that this object was last modified.</span></span> <br><span data-ttu-id="22bd8-152">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="22bd8-152">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="22bd8-153">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="22bd8-153">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
|<span data-ttu-id="22bd8-154">originId</span><span class="sxs-lookup"><span data-stu-id="22bd8-154">originId</span></span>|<span data-ttu-id="22bd8-155">String</span><span class="sxs-lookup"><span data-stu-id="22bd8-155">String</span></span>|<span data-ttu-id="22bd8-156">源系统中此环境的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="22bd8-156">The unique identifier of this environment in the origin system.</span></span>|
|<span data-ttu-id="22bd8-157">originSystem</span><span class="sxs-lookup"><span data-stu-id="22bd8-157">originSystem</span></span>|<span data-ttu-id="22bd8-158">String</span><span class="sxs-lookup"><span data-stu-id="22bd8-158">String</span></span>|<span data-ttu-id="22bd8-159">源系统中资源的类型，例如 `SharePointOnline` 。</span><span class="sxs-lookup"><span data-stu-id="22bd8-159">The type of the resource in the origin system such as `SharePointOnline`.</span></span> <span data-ttu-id="22bd8-160">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="22bd8-160">Supports `$filter`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22bd8-161">关系</span><span class="sxs-lookup"><span data-stu-id="22bd8-161">Relationships</span></span>
|<span data-ttu-id="22bd8-162">关系</span><span class="sxs-lookup"><span data-stu-id="22bd8-162">Relationship</span></span>|<span data-ttu-id="22bd8-163">类型</span><span class="sxs-lookup"><span data-stu-id="22bd8-163">Type</span></span>|<span data-ttu-id="22bd8-164">说明</span><span class="sxs-lookup"><span data-stu-id="22bd8-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22bd8-165">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="22bd8-165">accessPackageResources</span></span>|<span data-ttu-id="22bd8-166">[accessPackageResource](../resources/accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22bd8-166">[accessPackageResource](../resources/accesspackageresource.md) collection</span></span>|<span data-ttu-id="22bd8-167">只读。</span><span class="sxs-lookup"><span data-stu-id="22bd8-167">Read-only.</span></span> <span data-ttu-id="22bd8-168">必需。</span><span class="sxs-lookup"><span data-stu-id="22bd8-168">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22bd8-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22bd8-169">JSON representation</span></span>
<span data-ttu-id="22bd8-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22bd8-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceEnvironment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "originSystem": "String",
  "originId": "String",
  "isDefaultEnvironment": "Boolean",
  "connectionInfo": {
    "@odata.type": "microsoft.graph.connectionInfo"
  },
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```
