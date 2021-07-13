---
title: 更新 tenantCustomizedInformation
description: 更新 tenantCustomizedInformation 对象的属性。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c9d3c5a812364c5dd8999f89edd4c7ed411db0ab
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402086"
---
# <a name="update-tenantcustomizedinformation"></a><span data-ttu-id="8526a-103">更新 tenantCustomizedInformation</span><span class="sxs-lookup"><span data-stu-id="8526a-103">Update tenantCustomizedInformation</span></span>
<span data-ttu-id="8526a-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8526a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8526a-105">更新 [tenantCustomizedInformation 对象](../resources/managedtenants-tenantcustomizedinformation.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="8526a-105">Update the properties of a [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8526a-106">权限</span><span class="sxs-lookup"><span data-stu-id="8526a-106">Permissions</span></span>
<span data-ttu-id="8526a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8526a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8526a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8526a-109">Permission type</span></span>|<span data-ttu-id="8526a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8526a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8526a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8526a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8526a-112">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8526a-112">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="8526a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8526a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8526a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8526a-114">Not supported.</span></span>|
|<span data-ttu-id="8526a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8526a-115">Application</span></span>|<span data-ttu-id="8526a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8526a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8526a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8526a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
```

## <a name="request-headers"></a><span data-ttu-id="8526a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8526a-118">Request headers</span></span>
|<span data-ttu-id="8526a-119">名称</span><span class="sxs-lookup"><span data-stu-id="8526a-119">Name</span></span>|<span data-ttu-id="8526a-120">说明</span><span class="sxs-lookup"><span data-stu-id="8526a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8526a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8526a-121">Authorization</span></span>|<span data-ttu-id="8526a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8526a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8526a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8526a-124">Content-Type</span></span>|<span data-ttu-id="8526a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8526a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8526a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8526a-127">Request body</span></span>
<span data-ttu-id="8526a-128">在请求正文中，提供 [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8526a-128">In the request body, supply a JSON representation of the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object.</span></span>

<span data-ttu-id="8526a-129">下表显示更新 [tenantCustomizedInformation 时所需的属性](../resources/managedtenants-tenantcustomizedinformation.md)。</span><span class="sxs-lookup"><span data-stu-id="8526a-129">The following table shows the properties that are required when you update the [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md).</span></span>

|<span data-ttu-id="8526a-130">属性</span><span class="sxs-lookup"><span data-stu-id="8526a-130">Property</span></span>|<span data-ttu-id="8526a-131">类型</span><span class="sxs-lookup"><span data-stu-id="8526a-131">Type</span></span>|<span data-ttu-id="8526a-132">说明</span><span class="sxs-lookup"><span data-stu-id="8526a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8526a-133">id</span><span class="sxs-lookup"><span data-stu-id="8526a-133">id</span></span>|<span data-ttu-id="8526a-134">String</span><span class="sxs-lookup"><span data-stu-id="8526a-134">String</span></span>|<span data-ttu-id="8526a-135">托管Azure Active Directory租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="8526a-135">The Azure Active Directory tenant identifier for the managed tenant.</span></span>|
|<span data-ttu-id="8526a-136">tenantId</span><span class="sxs-lookup"><span data-stu-id="8526a-136">tenantId</span></span>|<span data-ttu-id="8526a-137">String</span><span class="sxs-lookup"><span data-stu-id="8526a-137">String</span></span>|<span data-ttu-id="8526a-138">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="8526a-138">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="8526a-139">contacts</span><span class="sxs-lookup"><span data-stu-id="8526a-139">contacts</span></span>|<span data-ttu-id="8526a-140">[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8526a-140">[microsoft.graph.managedTenants.tenantContactInformation](../resources/managedtenants-tenantcontactinformation.md) collection</span></span>|<span data-ttu-id="8526a-141">与托管租户关联的联系人集合。</span><span class="sxs-lookup"><span data-stu-id="8526a-141">The collection of contacts associated with the managed tenant.</span></span>|
|<span data-ttu-id="8526a-142">website</span><span class="sxs-lookup"><span data-stu-id="8526a-142">website</span></span>|<span data-ttu-id="8526a-143">String</span><span class="sxs-lookup"><span data-stu-id="8526a-143">String</span></span>|<span data-ttu-id="8526a-144">托管租户的网站。</span><span class="sxs-lookup"><span data-stu-id="8526a-144">The website for the managed tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="8526a-145">响应</span><span class="sxs-lookup"><span data-stu-id="8526a-145">Response</span></span>

<span data-ttu-id="8526a-146">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8526a-146">If successful, this method returns a `200 OK` response code and an updated [tenantCustomizedInformation](../resources/managedtenants-tenantcustomizedinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8526a-147">示例</span><span class="sxs-lookup"><span data-stu-id="8526a-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8526a-148">请求</span><span class="sxs-lookup"><span data-stu-id="8526a-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tenantcustomizedinformation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantsCustomizedInformation/{tenantCustomizedInformationId}
Content-Type: application/json
Content-length: 278

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "tenantId": "String",
  "contacts": [
    {
      "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
    }
  ],
  "website": "String"
}
```


### <a name="response"></a><span data-ttu-id="8526a-149">响应</span><span class="sxs-lookup"><span data-stu-id="8526a-149">Response</span></span>
><span data-ttu-id="8526a-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8526a-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantCustomizedInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenantCustomizedInformation",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "website": "https://www.fourthcoffee.com",
  "contacts": [
    {
      "name": "Sally",
      "email": "sally@fourthcoffee.com",
      "phone": "5558009731"
    },
    {
      "name": "Hector",
      "email": "hector@fourthcoffee.com",
      "phone": "5558009732"
    }
  ]
}
```
