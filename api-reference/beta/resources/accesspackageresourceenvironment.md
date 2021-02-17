---
title: accessPackageResourceEnvironment 资源类型
description: 访问包资源环境是资源所在的地理位置环境的引用。
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2f03e2c754ea09cdc797b71d4ef59372ac47ff9b
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272518"
---
# <a name="accesspackageresourceenvironment-resource-type"></a><span data-ttu-id="298fa-103">accessPackageResourceEnvironment 资源类型</span><span class="sxs-lookup"><span data-stu-id="298fa-103">accessPackageResourceEnvironment resource type</span></span>

<span data-ttu-id="298fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="298fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="298fa-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源环境是资源所在的地理位置环境的引用。</span><span class="sxs-lookup"><span data-stu-id="298fa-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource environment is a reference to the geolocation environment in which a resource is located.</span></span> <span data-ttu-id="298fa-106">此环境自动作为 Azure AD 权利管理的一部分提供。</span><span class="sxs-lookup"><span data-stu-id="298fa-106">This environment is automatically provided as part of Azure AD Entitlement Management.</span></span> <span data-ttu-id="298fa-107">此 API 仅适用于多地理位置 SharePoint Online 网站。</span><span class="sxs-lookup"><span data-stu-id="298fa-107">The API is only applicable to Multi-Geo SharePoint Online sites.</span></span>

## <a name="methods"></a><span data-ttu-id="298fa-108">Methods</span><span class="sxs-lookup"><span data-stu-id="298fa-108">Methods</span></span>
|<span data-ttu-id="298fa-109">方法</span><span class="sxs-lookup"><span data-stu-id="298fa-109">Method</span></span>|<span data-ttu-id="298fa-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="298fa-110">Return type</span></span>|<span data-ttu-id="298fa-111">说明</span><span class="sxs-lookup"><span data-stu-id="298fa-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="298fa-112">列出 accessPackageResourceEnvironments</span><span class="sxs-lookup"><span data-stu-id="298fa-112">List accessPackageResourceEnvironments</span></span>](../api/accesspackageresourceenvironment-list.md)|<span data-ttu-id="298fa-113">[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="298fa-113">[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection</span></span>|<span data-ttu-id="298fa-114">检索 [accessPackageResourceEnvironment 对象](../resources/accesspackageresourceenvironment.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="298fa-114">Retrieve a list of [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) objects.</span></span>|
|[<span data-ttu-id="298fa-115">获取 accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="298fa-115">Get accessPackageResourceEnvironment</span></span>](../api/accesspackageresourceenvironment-get.md)|[<span data-ttu-id="298fa-116">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="298fa-116">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="298fa-117">读取 [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="298fa-117">Read the properties and relationships of an [accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="298fa-118">属性</span><span class="sxs-lookup"><span data-stu-id="298fa-118">Properties</span></span>
|<span data-ttu-id="298fa-119">属性</span><span class="sxs-lookup"><span data-stu-id="298fa-119">Property</span></span>|<span data-ttu-id="298fa-120">类型</span><span class="sxs-lookup"><span data-stu-id="298fa-120">Type</span></span>|<span data-ttu-id="298fa-121">说明</span><span class="sxs-lookup"><span data-stu-id="298fa-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="298fa-122">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="298fa-122">connectionInfo</span></span>|[<span data-ttu-id="298fa-123">connectionInfo</span><span class="sxs-lookup"><span data-stu-id="298fa-123">connectionInfo</span></span>](../resources/connectioninfo.md)|<span data-ttu-id="298fa-124">用于连接到资源的环境的连接信息。</span><span class="sxs-lookup"><span data-stu-id="298fa-124">Connection information of an environment used to connect to a resource.</span></span> |
|<span data-ttu-id="298fa-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="298fa-125">createdBy</span></span>|<span data-ttu-id="298fa-126">String</span><span class="sxs-lookup"><span data-stu-id="298fa-126">String</span></span>|<span data-ttu-id="298fa-127">创建显示名称的用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="298fa-127">The display name of the user that created this object.</span></span>|
|<span data-ttu-id="298fa-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="298fa-128">createdDateTime</span></span>|<span data-ttu-id="298fa-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="298fa-129">DateTimeOffset</span></span>|<span data-ttu-id="298fa-130">创建此对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="298fa-130">The date and time that this object was created.</span></span> <br><span data-ttu-id="298fa-131">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="298fa-131">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="298fa-132">例如，2014 年 1 月 1 日午夜 UTC 为 `'2014-01-01T00:00:00Z'` 。</span><span class="sxs-lookup"><span data-stu-id="298fa-132">For example, midnight UTC on Jan 1, 2014 is `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="298fa-133">description</span><span class="sxs-lookup"><span data-stu-id="298fa-133">description</span></span>|<span data-ttu-id="298fa-134">String</span><span class="sxs-lookup"><span data-stu-id="298fa-134">String</span></span>|<span data-ttu-id="298fa-135">此 *accessPackageResourceEnvironment 对象的* 说明。</span><span class="sxs-lookup"><span data-stu-id="298fa-135">The description of this *accessPackageResourceEnvironment* object.</span></span>|
|<span data-ttu-id="298fa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="298fa-136">displayName</span></span>|<span data-ttu-id="298fa-137">String</span><span class="sxs-lookup"><span data-stu-id="298fa-137">String</span></span>|<span data-ttu-id="298fa-138">此显示名称对象的对象。</span><span class="sxs-lookup"><span data-stu-id="298fa-138">The display name of this object.</span></span>|
|<span data-ttu-id="298fa-139">id</span><span class="sxs-lookup"><span data-stu-id="298fa-139">id</span></span>|<span data-ttu-id="298fa-140">String</span><span class="sxs-lookup"><span data-stu-id="298fa-140">String</span></span>|<span data-ttu-id="298fa-141">系统分配的对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="298fa-141">The system-assigned unique identifier of the object.</span></span>|
|<span data-ttu-id="298fa-142">isDefaultEnvironment</span><span class="sxs-lookup"><span data-stu-id="298fa-142">isDefaultEnvironment</span></span>|<span data-ttu-id="298fa-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="298fa-143">Boolean</span></span>|<span data-ttu-id="298fa-144">确定这是否是默认环境。</span><span class="sxs-lookup"><span data-stu-id="298fa-144">Determines whether this is default environment or not.</span></span> <span data-ttu-id="298fa-145">它设置为 `true` 所有静态源系统，如 Azure AD 组和 Azure AD 应用程序。</span><span class="sxs-lookup"><span data-stu-id="298fa-145">It is set to `true` for all static origin systems, such as Azure AD groups and Azure AD Applications.</span></span>|
|<span data-ttu-id="298fa-146">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="298fa-146">modifiedBy</span></span>|<span data-ttu-id="298fa-147">String</span><span class="sxs-lookup"><span data-stu-id="298fa-147">String</span></span>|<span data-ttu-id="298fa-148">最后显示名称修改此对象的实体的属性。</span><span class="sxs-lookup"><span data-stu-id="298fa-148">The display name of the entity that last modified this object.</span></span>|
|<span data-ttu-id="298fa-149">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="298fa-149">modifiedDateTime</span></span>|<span data-ttu-id="298fa-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="298fa-150">DateTimeOffset</span></span>|<span data-ttu-id="298fa-151">上次修改此对象的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="298fa-151">The date and time that this object was last modified.</span></span> <br><span data-ttu-id="298fa-152">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="298fa-152">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="298fa-153">例如，2014 年 1 月 1 日午夜 UTC 为 `'2014-01-01T00:00:00Z'` 。</span><span class="sxs-lookup"><span data-stu-id="298fa-153">For example, midnight UTC on Jan 1, 2014 is `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="298fa-154">originId</span><span class="sxs-lookup"><span data-stu-id="298fa-154">originId</span></span>|<span data-ttu-id="298fa-155">String</span><span class="sxs-lookup"><span data-stu-id="298fa-155">String</span></span>|<span data-ttu-id="298fa-156">源系统中此环境的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="298fa-156">The unique identifier of this environment in the origin system.</span></span>|
|<span data-ttu-id="298fa-157">originSystem</span><span class="sxs-lookup"><span data-stu-id="298fa-157">originSystem</span></span>|<span data-ttu-id="298fa-158">String</span><span class="sxs-lookup"><span data-stu-id="298fa-158">String</span></span>|<span data-ttu-id="298fa-159">源系统中资源的类型，例如 `SharePointOnline` 。</span><span class="sxs-lookup"><span data-stu-id="298fa-159">The type of the resource in the origin system such as `SharePointOnline`.</span></span> <span data-ttu-id="298fa-160">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="298fa-160">Supports `$filter`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="298fa-161">关系</span><span class="sxs-lookup"><span data-stu-id="298fa-161">Relationships</span></span>
|<span data-ttu-id="298fa-162">关系</span><span class="sxs-lookup"><span data-stu-id="298fa-162">Relationship</span></span>|<span data-ttu-id="298fa-163">类型</span><span class="sxs-lookup"><span data-stu-id="298fa-163">Type</span></span>|<span data-ttu-id="298fa-164">说明</span><span class="sxs-lookup"><span data-stu-id="298fa-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="298fa-165">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="298fa-165">accessPackageResources</span></span>|<span data-ttu-id="298fa-166">[accessPackageResource](../resources/accesspackageresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="298fa-166">[accessPackageResource](../resources/accesspackageresource.md) collection</span></span>|<span data-ttu-id="298fa-167">只读。</span><span class="sxs-lookup"><span data-stu-id="298fa-167">Read-only.</span></span> <span data-ttu-id="298fa-168">必需。</span><span class="sxs-lookup"><span data-stu-id="298fa-168">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="298fa-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="298fa-169">JSON representation</span></span>
<span data-ttu-id="298fa-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="298fa-170">The following is a JSON representation of the resource.</span></span>
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
