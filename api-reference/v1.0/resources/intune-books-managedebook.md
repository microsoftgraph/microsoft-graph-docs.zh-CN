---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
ms.openlocfilehash: 427582977558254561b219dff2392f01ced4f53d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010904"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="9af6c-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="9af6c-103">managedEBook resource type</span></span>

> <span data-ttu-id="9af6c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9af6c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9af6c-105">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="9af6c-105">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="9af6c-106">方法</span><span class="sxs-lookup"><span data-stu-id="9af6c-106">Methods</span></span>
|<span data-ttu-id="9af6c-107">方法</span><span class="sxs-lookup"><span data-stu-id="9af6c-107">Method</span></span>|<span data-ttu-id="9af6c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9af6c-108">Return Type</span></span>|<span data-ttu-id="9af6c-109">说明</span><span class="sxs-lookup"><span data-stu-id="9af6c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9af6c-110">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="9af6c-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="9af6c-111">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9af6c-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="9af6c-112">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9af6c-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="9af6c-113">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="9af6c-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="9af6c-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="9af6c-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="9af6c-115">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9af6c-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="9af6c-116">assign 操作</span><span class="sxs-lookup"><span data-stu-id="9af6c-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="9af6c-117">无</span><span class="sxs-lookup"><span data-stu-id="9af6c-117">None</span></span>|<span data-ttu-id="9af6c-118">尚未记录</span><span class="sxs-lookup"><span data-stu-id="9af6c-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9af6c-119">属性</span><span class="sxs-lookup"><span data-stu-id="9af6c-119">Properties</span></span>
|<span data-ttu-id="9af6c-120">属性</span><span class="sxs-lookup"><span data-stu-id="9af6c-120">Property</span></span>|<span data-ttu-id="9af6c-121">类型</span><span class="sxs-lookup"><span data-stu-id="9af6c-121">Type</span></span>|<span data-ttu-id="9af6c-122">说明</span><span class="sxs-lookup"><span data-stu-id="9af6c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9af6c-123">id</span><span class="sxs-lookup"><span data-stu-id="9af6c-123">id</span></span>|<span data-ttu-id="9af6c-124">String</span><span class="sxs-lookup"><span data-stu-id="9af6c-124">String</span></span>|<span data-ttu-id="9af6c-125">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9af6c-125">Key of the entity.</span></span>|
|<span data-ttu-id="9af6c-126">displayName</span><span class="sxs-lookup"><span data-stu-id="9af6c-126">displayName</span></span>|<span data-ttu-id="9af6c-127">String</span><span class="sxs-lookup"><span data-stu-id="9af6c-127">String</span></span>|<span data-ttu-id="9af6c-128">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="9af6c-128">Name of the eBook.</span></span>|
|<span data-ttu-id="9af6c-129">description</span><span class="sxs-lookup"><span data-stu-id="9af6c-129">description</span></span>|<span data-ttu-id="9af6c-130">String</span><span class="sxs-lookup"><span data-stu-id="9af6c-130">String</span></span>|<span data-ttu-id="9af6c-131">说明。</span><span class="sxs-lookup"><span data-stu-id="9af6c-131">Description.</span></span>|
|<span data-ttu-id="9af6c-132">publisher</span><span class="sxs-lookup"><span data-stu-id="9af6c-132">publisher</span></span>|<span data-ttu-id="9af6c-133">String</span><span class="sxs-lookup"><span data-stu-id="9af6c-133">String</span></span>|<span data-ttu-id="9af6c-134">发布者。</span><span class="sxs-lookup"><span data-stu-id="9af6c-134">Publisher.</span></span>|
|<span data-ttu-id="9af6c-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="9af6c-135">publishedDateTime</span></span>|<span data-ttu-id="9af6c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9af6c-136">DateTimeOffset</span></span>|<span data-ttu-id="9af6c-137">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9af6c-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="9af6c-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="9af6c-138">largeCover</span></span>|[<span data-ttu-id="9af6c-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9af6c-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9af6c-140">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="9af6c-140">Book cover.</span></span>|
|<span data-ttu-id="9af6c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9af6c-141">createdDateTime</span></span>|<span data-ttu-id="9af6c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9af6c-142">DateTimeOffset</span></span>|<span data-ttu-id="9af6c-143">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9af6c-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="9af6c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9af6c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="9af6c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9af6c-145">DateTimeOffset</span></span>|<span data-ttu-id="9af6c-146">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9af6c-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="9af6c-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9af6c-147">informationUrl</span></span>|<span data-ttu-id="9af6c-148">String</span><span class="sxs-lookup"><span data-stu-id="9af6c-148">String</span></span>|<span data-ttu-id="9af6c-149">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="9af6c-149">The more information Url.</span></span>|
|<span data-ttu-id="9af6c-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9af6c-150">privacyInformationUrl</span></span>|<span data-ttu-id="9af6c-151">String</span><span class="sxs-lookup"><span data-stu-id="9af6c-151">String</span></span>|<span data-ttu-id="9af6c-152">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="9af6c-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9af6c-153">关系</span><span class="sxs-lookup"><span data-stu-id="9af6c-153">Relationships</span></span>
|<span data-ttu-id="9af6c-154">关系</span><span class="sxs-lookup"><span data-stu-id="9af6c-154">Relationship</span></span>|<span data-ttu-id="9af6c-155">类型</span><span class="sxs-lookup"><span data-stu-id="9af6c-155">Type</span></span>|<span data-ttu-id="9af6c-156">说明</span><span class="sxs-lookup"><span data-stu-id="9af6c-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9af6c-157">assignments</span><span class="sxs-lookup"><span data-stu-id="9af6c-157">assignments</span></span>|<span data-ttu-id="9af6c-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9af6c-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="9af6c-159">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="9af6c-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="9af6c-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="9af6c-160">installSummary</span></span>|[<span data-ttu-id="9af6c-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="9af6c-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="9af6c-162">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="9af6c-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="9af6c-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="9af6c-163">deviceStates</span></span>|<span data-ttu-id="9af6c-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9af6c-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="9af6c-165">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="9af6c-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="9af6c-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="9af6c-166">userStateSummary</span></span>|<span data-ttu-id="9af6c-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9af6c-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="9af6c-168">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="9af6c-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9af6c-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9af6c-169">JSON Representation</span></span>
<span data-ttu-id="9af6c-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9af6c-170">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



