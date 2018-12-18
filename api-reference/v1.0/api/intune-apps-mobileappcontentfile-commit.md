---
title: commit 操作
description: 提交给定应用的文件。
author: tfitzmac
ms.openlocfilehash: 728cbaeb431fd6f3f9b27b64d118a603bbf9347d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345435"
---
# <a name="commit-action"></a><span data-ttu-id="0b656-103">commit 操作</span><span class="sxs-lookup"><span data-stu-id="0b656-103">commit action</span></span>

> <span data-ttu-id="0b656-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b656-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b656-105">提交给定应用的文件。</span><span class="sxs-lookup"><span data-stu-id="0b656-105">Commits a file of a given app.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b656-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b656-106">Prerequisites</span></span>
<span data-ttu-id="0b656-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0b656-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b656-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b656-109">Permission type</span></span>|<span data-ttu-id="0b656-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b656-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b656-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b656-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b656-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b656-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b656-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b656-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b656-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b656-114">Not supported.</span></span>|
|<span data-ttu-id="0b656-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b656-115">Application</span></span>|<span data-ttu-id="0b656-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b656-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b656-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b656-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a><span data-ttu-id="0b656-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b656-118">Request headers</span></span>
|<span data-ttu-id="0b656-119">标头</span><span class="sxs-lookup"><span data-stu-id="0b656-119">Header</span></span>|<span data-ttu-id="0b656-120">值</span><span class="sxs-lookup"><span data-stu-id="0b656-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b656-121">授权</span><span class="sxs-lookup"><span data-stu-id="0b656-121">Authorization</span></span>|<span data-ttu-id="0b656-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b656-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b656-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0b656-123">Accept</span></span>|<span data-ttu-id="0b656-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0b656-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b656-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b656-125">Request body</span></span>
<span data-ttu-id="0b656-126">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b656-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="0b656-127">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="0b656-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="0b656-128">属性</span><span class="sxs-lookup"><span data-stu-id="0b656-128">Property</span></span>|<span data-ttu-id="0b656-129">类型</span><span class="sxs-lookup"><span data-stu-id="0b656-129">Type</span></span>|<span data-ttu-id="0b656-130">说明</span><span class="sxs-lookup"><span data-stu-id="0b656-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b656-131">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="0b656-131">fileEncryptionInfo</span></span>|[<span data-ttu-id="0b656-132">fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="0b656-132">fileEncryptionInfo</span></span>](../resources/intune-apps-fileencryptioninfo.md)|<span data-ttu-id="0b656-133">文件加密信息参数密钥。</span><span class="sxs-lookup"><span data-stu-id="0b656-133">File encryption info parameter key.</span></span>|



## <a name="response"></a><span data-ttu-id="0b656-134">响应</span><span class="sxs-lookup"><span data-stu-id="0b656-134">Response</span></span>
<span data-ttu-id="0b656-135">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0b656-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0b656-136">示例</span><span class="sxs-lookup"><span data-stu-id="0b656-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b656-137">请求</span><span class="sxs-lookup"><span data-stu-id="0b656-137">Request</span></span>
<span data-ttu-id="0b656-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b656-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

Content-type: application/json
Content-length: 399

{
  "fileEncryptionInfo": {
    "@odata.type": "microsoft.graph.fileEncryptionInfo",
    "encryptionKey": "ZW5jcnlwdGlvbktleQ==",
    "initializationVector": "aW5pdGlhbGl6YXRpb25WZWN0b3I=",
    "mac": "bWFj",
    "macKey": "bWFjS2V5",
    "profileIdentifier": "Profile Identifier value",
    "fileDigest": "ZmlsZURpZ2VzdA==",
    "fileDigestAlgorithm": "File Digest Algorithm value"
  }
}
```

### <a name="response"></a><span data-ttu-id="0b656-139">响应</span><span class="sxs-lookup"><span data-stu-id="0b656-139">Response</span></span>
<span data-ttu-id="0b656-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b656-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



