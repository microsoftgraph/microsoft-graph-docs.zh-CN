---
title: 更新 roleScopeTag
description: 更新 roleScopeTag 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3670850bb0a9b3907b02c3e48d893b35ce7fcbb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527271"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="12b7c-103">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="12b7c-103">Update roleScopeTag</span></span>

> <span data-ttu-id="12b7c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12b7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12b7c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12b7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12b7c-106">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="12b7c-106">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12b7c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="12b7c-107">Prerequisites</span></span>
<span data-ttu-id="12b7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12b7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12b7c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="12b7c-110">Permission type</span></span>|<span data-ttu-id="12b7c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="12b7c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12b7c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12b7c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12b7c-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12b7c-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="12b7c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12b7c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12b7c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="12b7c-115">Not supported.</span></span>|
|<span data-ttu-id="12b7c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="12b7c-116">Application</span></span>|<span data-ttu-id="12b7c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="12b7c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12b7c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12b7c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="12b7c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="12b7c-119">Request headers</span></span>
|<span data-ttu-id="12b7c-120">标头</span><span class="sxs-lookup"><span data-stu-id="12b7c-120">Header</span></span>|<span data-ttu-id="12b7c-121">值</span><span class="sxs-lookup"><span data-stu-id="12b7c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12b7c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12b7c-122">Authorization</span></span>|<span data-ttu-id="12b7c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="12b7c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12b7c-124">接受</span><span class="sxs-lookup"><span data-stu-id="12b7c-124">Accept</span></span>|<span data-ttu-id="12b7c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12b7c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12b7c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="12b7c-126">Request body</span></span>
<span data-ttu-id="12b7c-127">在请求正文中, 提供[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12b7c-127">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="12b7c-128">下表显示创建[roleScopeTag](../resources/intune-rbac-rolescopetag.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="12b7c-128">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="12b7c-129">属性</span><span class="sxs-lookup"><span data-stu-id="12b7c-129">Property</span></span>|<span data-ttu-id="12b7c-130">类型</span><span class="sxs-lookup"><span data-stu-id="12b7c-130">Type</span></span>|<span data-ttu-id="12b7c-131">说明</span><span class="sxs-lookup"><span data-stu-id="12b7c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12b7c-132">id</span><span class="sxs-lookup"><span data-stu-id="12b7c-132">id</span></span>|<span data-ttu-id="12b7c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="12b7c-133">String</span></span>|<span data-ttu-id="12b7c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="12b7c-134">Key of the entity.</span></span> <span data-ttu-id="12b7c-135">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="12b7c-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="12b7c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="12b7c-136">displayName</span></span>|<span data-ttu-id="12b7c-137">String</span><span class="sxs-lookup"><span data-stu-id="12b7c-137">String</span></span>|<span data-ttu-id="12b7c-138">角色范围标记的显示名称或友好名称。</span><span class="sxs-lookup"><span data-stu-id="12b7c-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="12b7c-139">description</span><span class="sxs-lookup"><span data-stu-id="12b7c-139">description</span></span>|<span data-ttu-id="12b7c-140">String</span><span class="sxs-lookup"><span data-stu-id="12b7c-140">String</span></span>|<span data-ttu-id="12b7c-141">角色范围标记的说明。</span><span class="sxs-lookup"><span data-stu-id="12b7c-141">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="12b7c-142">响应</span><span class="sxs-lookup"><span data-stu-id="12b7c-142">Response</span></span>
<span data-ttu-id="12b7c-143">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="12b7c-143">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12b7c-144">示例</span><span class="sxs-lookup"><span data-stu-id="12b7c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="12b7c-145">请求</span><span class="sxs-lookup"><span data-stu-id="12b7c-145">Request</span></span>
<span data-ttu-id="12b7c-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="12b7c-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="12b7c-147">响应</span><span class="sxs-lookup"><span data-stu-id="12b7c-147">Response</span></span>
<span data-ttu-id="12b7c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="12b7c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





