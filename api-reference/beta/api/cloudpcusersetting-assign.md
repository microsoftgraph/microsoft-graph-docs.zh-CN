---
title: cloudPcUserSetting：assign
description: 将云电脑用户设置分配给用户组。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 66da3f668cc25807ece4a63e51dabe3f5436cf7d
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082088"
---
# <a name="cloudpcusersetting-assign"></a><span data-ttu-id="a827c-103">cloudPcUserSetting：assign</span><span class="sxs-lookup"><span data-stu-id="a827c-103">cloudPcUserSetting: assign</span></span>

<span data-ttu-id="a827c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a827c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a827c-105">将 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 分配给用户组。</span><span class="sxs-lookup"><span data-stu-id="a827c-105">Assign a [cloudPcUserSetting](../resources/cloudpcusersetting.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="a827c-106">权限</span><span class="sxs-lookup"><span data-stu-id="a827c-106">Permissions</span></span>

<span data-ttu-id="a827c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a827c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a827c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a827c-109">Permission type</span></span>|<span data-ttu-id="a827c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a827c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a827c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a827c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a827c-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a827c-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="a827c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a827c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a827c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a827c-114">Not supported.</span></span>|
|<span data-ttu-id="a827c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a827c-115">Application</span></span>|<span data-ttu-id="a827c-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a827c-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a827c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a827c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="a827c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a827c-118">Request headers</span></span>

|<span data-ttu-id="a827c-119">名称</span><span class="sxs-lookup"><span data-stu-id="a827c-119">Name</span></span>|<span data-ttu-id="a827c-120">说明</span><span class="sxs-lookup"><span data-stu-id="a827c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a827c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a827c-121">Authorization</span></span>|<span data-ttu-id="a827c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a827c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a827c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a827c-124">Content-Type</span></span>|<span data-ttu-id="a827c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a827c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a827c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a827c-127">Request body</span></span>

<span data-ttu-id="a827c-128">在请求正文中，提供 [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a827c-128">In the request body, supply a JSON representation of the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) object.</span></span>

|<span data-ttu-id="a827c-129">参数</span><span class="sxs-lookup"><span data-stu-id="a827c-129">Parameter</span></span>|<span data-ttu-id="a827c-130">类型</span><span class="sxs-lookup"><span data-stu-id="a827c-130">Type</span></span>|<span data-ttu-id="a827c-131">说明</span><span class="sxs-lookup"><span data-stu-id="a827c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a827c-132">assignments</span><span class="sxs-lookup"><span data-stu-id="a827c-132">assignments</span></span>|<span data-ttu-id="a827c-133">[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a827c-133">[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) collection</span></span> | <span data-ttu-id="a827c-134">要分配给相应目标组的云电脑用户设置资源的集合。</span><span class="sxs-lookup"><span data-stu-id="a827c-134">The collection of cloud PC user setting resources each to be assigned to the corresponding target group.</span></span> <span data-ttu-id="a827c-135">目前Microsoft 365 Azure AD 中的安全组和安全组。</span><span class="sxs-lookup"><span data-stu-id="a827c-135">Only Microsoft 365 groups and security groups in Azure AD are currently supported.</span></span> |

## <a name="response"></a><span data-ttu-id="a827c-136">响应</span><span class="sxs-lookup"><span data-stu-id="a827c-136">Response</span></span>

<span data-ttu-id="a827c-137">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a827c-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a827c-138">示例</span><span class="sxs-lookup"><span data-stu-id="a827c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a827c-139">请求</span><span class="sxs-lookup"><span data-stu-id="a827c-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "cloudpcusersetting_assign"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff/assign
Content-Type: application/json
Content-length: 254

{
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="a827c-140">响应</span><span class="sxs-lookup"><span data-stu-id="a827c-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
