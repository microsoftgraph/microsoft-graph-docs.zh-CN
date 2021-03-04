---
title: microsoftAuthenticatorAuthenticationMethod 资源类型
description: 注册到用户的 Microsoft Authenticator 应用的表示形式。 Microsoft Authenticator 是一种身份验证方法。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7438ca72a4f5d4063eec0444d3b0028237083d9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444138"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a><span data-ttu-id="3ed0d-104">microsoftAuthenticatorAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ed0d-104">microsoftAuthenticatorAuthenticationMethod resource type</span></span>

<span data-ttu-id="3ed0d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ed0d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ed0d-106">注册到用户的 Microsoft Authenticator 应用的表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-106">A representation of the Microsoft Authenticator app registered to a user.</span></span> <span data-ttu-id="3ed0d-107">Microsoft Authenticator 是一种身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-107">Microsoft Authenticator is an authentication method.</span></span>

<span data-ttu-id="3ed0d-108">继承自 [authenticationMethod](../resources/authenticationmethod.md)。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3ed0d-109">Methods</span><span class="sxs-lookup"><span data-stu-id="3ed0d-109">Methods</span></span>
|<span data-ttu-id="3ed0d-110">方法</span><span class="sxs-lookup"><span data-stu-id="3ed0d-110">Method</span></span>|<span data-ttu-id="3ed0d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3ed0d-111">Return type</span></span>|<span data-ttu-id="3ed0d-112">说明</span><span class="sxs-lookup"><span data-stu-id="3ed0d-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3ed0d-113">列出 microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="3ed0d-113">List microsoftAuthenticatorAuthenticationMethods</span></span>](../api/microsoftauthenticatorauthenticationmethod-list.md)|<span data-ttu-id="3ed0d-114">[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ed0d-114">[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="3ed0d-115">获取 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-115">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="3ed0d-116">获取 microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ed0d-116">Get microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-get.md)|[<span data-ttu-id="3ed0d-117">microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ed0d-117">microsoftAuthenticatorAuthenticationMethod</span></span>](../resources/microsoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="3ed0d-118">读取 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-118">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="3ed0d-119">删除 microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ed0d-119">Delete microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-delete.md)|<span data-ttu-id="3ed0d-120">无</span><span class="sxs-lookup"><span data-stu-id="3ed0d-120">None</span></span>|<span data-ttu-id="3ed0d-121">删除 [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-121">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ed0d-122">属性</span><span class="sxs-lookup"><span data-stu-id="3ed0d-122">Properties</span></span>
|<span data-ttu-id="3ed0d-123">属性</span><span class="sxs-lookup"><span data-stu-id="3ed0d-123">Property</span></span>|<span data-ttu-id="3ed0d-124">类型</span><span class="sxs-lookup"><span data-stu-id="3ed0d-124">Type</span></span>|<span data-ttu-id="3ed0d-125">说明</span><span class="sxs-lookup"><span data-stu-id="3ed0d-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ed0d-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ed0d-126">createdDateTime</span></span>|<span data-ttu-id="3ed0d-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ed0d-127">DateTimeOffset</span></span>|<span data-ttu-id="3ed0d-128">此应用程序的注册日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-128">The date and time that this app was registered.</span></span> <span data-ttu-id="3ed0d-129">如果设备未注册无密码电话登录，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-129">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|
|<span data-ttu-id="3ed0d-130">displayName</span><span class="sxs-lookup"><span data-stu-id="3ed0d-130">displayName</span></span>|<span data-ttu-id="3ed0d-131">String</span><span class="sxs-lookup"><span data-stu-id="3ed0d-131">String</span></span>|<span data-ttu-id="3ed0d-132">注册此应用的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-132">The name of the device on which this app is registered.</span></span>|
|<span data-ttu-id="3ed0d-133">id</span><span class="sxs-lookup"><span data-stu-id="3ed0d-133">id</span></span>|<span data-ttu-id="3ed0d-134">String</span><span class="sxs-lookup"><span data-stu-id="3ed0d-134">String</span></span>|<span data-ttu-id="3ed0d-135">此身份验证方法的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-135">A unique identifier for this authentication method.</span></span> <span data-ttu-id="3ed0d-136">继承自 [authenticationMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="3ed0d-136">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="3ed0d-137">deviceTag</span><span class="sxs-lookup"><span data-stu-id="3ed0d-137">deviceTag</span></span>|<span data-ttu-id="3ed0d-138">String</span><span class="sxs-lookup"><span data-stu-id="3ed0d-138">String</span></span>|<span data-ttu-id="3ed0d-139">包含应用元数据的标记。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-139">Tags containing app metadata.</span></span>|
|<span data-ttu-id="3ed0d-140">phoneAppVersion</span><span class="sxs-lookup"><span data-stu-id="3ed0d-140">phoneAppVersion</span></span>|<span data-ttu-id="3ed0d-141">String</span><span class="sxs-lookup"><span data-stu-id="3ed0d-141">String</span></span>|<span data-ttu-id="3ed0d-142">Authenticator 应用的此实例的数字版本。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-142">Numerical version of this instance of the Authenticator app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ed0d-143">关系</span><span class="sxs-lookup"><span data-stu-id="3ed0d-143">Relationships</span></span>
|<span data-ttu-id="3ed0d-144">关系</span><span class="sxs-lookup"><span data-stu-id="3ed0d-144">Relationship</span></span>|<span data-ttu-id="3ed0d-145">类型</span><span class="sxs-lookup"><span data-stu-id="3ed0d-145">Type</span></span>|<span data-ttu-id="3ed0d-146">说明</span><span class="sxs-lookup"><span data-stu-id="3ed0d-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ed0d-147">设备</span><span class="sxs-lookup"><span data-stu-id="3ed0d-147">device</span></span>|[<span data-ttu-id="3ed0d-148">设备</span><span class="sxs-lookup"><span data-stu-id="3ed0d-148">device</span></span>](../resources/device.md)|<span data-ttu-id="3ed0d-149">Microsoft Authenticator 所在的已注册设备。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-149">The registered device on which Microsoft Authenticator resides.</span></span> <span data-ttu-id="3ed0d-150">如果设备未注册无密码电话登录，则此属性为 null。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-150">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ed0d-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ed0d-151">JSON representation</span></span>
<span data-ttu-id="3ed0d-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ed0d-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "deviceTag": "String",
  "phoneAppVersion": "String",
  "createdDateTime": "DateTimeOffset"
}
```
