---
title: managedEBook 资源类型
description: 包含托管电子书基属性的抽象类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24a8619d92eee6c666b7126a84895b14e0404755
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156033"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="f94b7-103">managedEBook 资源类型</span><span class="sxs-lookup"><span data-stu-id="f94b7-103">managedEBook resource type</span></span>

> <span data-ttu-id="f94b7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f94b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f94b7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f94b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f94b7-106">包含托管电子书基属性的抽象类。</span><span class="sxs-lookup"><span data-stu-id="f94b7-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="f94b7-107">方法</span><span class="sxs-lookup"><span data-stu-id="f94b7-107">Methods</span></span>
|<span data-ttu-id="f94b7-108">方法</span><span class="sxs-lookup"><span data-stu-id="f94b7-108">Method</span></span>|<span data-ttu-id="f94b7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f94b7-109">Return Type</span></span>|<span data-ttu-id="f94b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="f94b7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f94b7-111">List managedEBooks</span><span class="sxs-lookup"><span data-stu-id="f94b7-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="f94b7-112">[managedEBook](../resources/intune-books-managedebook.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f94b7-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="f94b7-113">列出 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f94b7-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="f94b7-114">Get managedEBook</span><span class="sxs-lookup"><span data-stu-id="f94b7-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="f94b7-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="f94b7-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="f94b7-116">读取 [managedEBook](../resources/intune-books-managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f94b7-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="f94b7-117">assign 操作</span><span class="sxs-lookup"><span data-stu-id="f94b7-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="f94b7-118">无</span><span class="sxs-lookup"><span data-stu-id="f94b7-118">None</span></span>|<span data-ttu-id="f94b7-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f94b7-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f94b7-120">属性</span><span class="sxs-lookup"><span data-stu-id="f94b7-120">Properties</span></span>
|<span data-ttu-id="f94b7-121">属性</span><span class="sxs-lookup"><span data-stu-id="f94b7-121">Property</span></span>|<span data-ttu-id="f94b7-122">类型</span><span class="sxs-lookup"><span data-stu-id="f94b7-122">Type</span></span>|<span data-ttu-id="f94b7-123">说明</span><span class="sxs-lookup"><span data-stu-id="f94b7-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f94b7-124">id</span><span class="sxs-lookup"><span data-stu-id="f94b7-124">id</span></span>|<span data-ttu-id="f94b7-125">字符串</span><span class="sxs-lookup"><span data-stu-id="f94b7-125">String</span></span>|<span data-ttu-id="f94b7-126">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f94b7-126">Key of the entity.</span></span>|
|<span data-ttu-id="f94b7-127">displayName</span><span class="sxs-lookup"><span data-stu-id="f94b7-127">displayName</span></span>|<span data-ttu-id="f94b7-128">String</span><span class="sxs-lookup"><span data-stu-id="f94b7-128">String</span></span>|<span data-ttu-id="f94b7-129">电子书的名称。</span><span class="sxs-lookup"><span data-stu-id="f94b7-129">Name of the eBook.</span></span>|
|<span data-ttu-id="f94b7-130">description</span><span class="sxs-lookup"><span data-stu-id="f94b7-130">description</span></span>|<span data-ttu-id="f94b7-131">字符串</span><span class="sxs-lookup"><span data-stu-id="f94b7-131">String</span></span>|<span data-ttu-id="f94b7-132">说明。</span><span class="sxs-lookup"><span data-stu-id="f94b7-132">Description.</span></span>|
|<span data-ttu-id="f94b7-133">publisher</span><span class="sxs-lookup"><span data-stu-id="f94b7-133">publisher</span></span>|<span data-ttu-id="f94b7-134">String</span><span class="sxs-lookup"><span data-stu-id="f94b7-134">String</span></span>|<span data-ttu-id="f94b7-135">发布者。</span><span class="sxs-lookup"><span data-stu-id="f94b7-135">Publisher.</span></span>|
|<span data-ttu-id="f94b7-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="f94b7-136">publishedDateTime</span></span>|<span data-ttu-id="f94b7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f94b7-137">DateTimeOffset</span></span>|<span data-ttu-id="f94b7-138">电子书的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f94b7-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="f94b7-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="f94b7-139">largeCover</span></span>|[<span data-ttu-id="f94b7-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f94b7-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f94b7-141">书籍封面。</span><span class="sxs-lookup"><span data-stu-id="f94b7-141">Book cover.</span></span>|
|<span data-ttu-id="f94b7-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f94b7-142">createdDateTime</span></span>|<span data-ttu-id="f94b7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f94b7-143">DateTimeOffset</span></span>|<span data-ttu-id="f94b7-144">电子书文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f94b7-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="f94b7-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f94b7-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f94b7-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f94b7-146">DateTimeOffset</span></span>|<span data-ttu-id="f94b7-147">上次修改电子书的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f94b7-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="f94b7-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f94b7-148">informationUrl</span></span>|<span data-ttu-id="f94b7-149">String</span><span class="sxs-lookup"><span data-stu-id="f94b7-149">String</span></span>|<span data-ttu-id="f94b7-150">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="f94b7-150">The more information Url.</span></span>|
|<span data-ttu-id="f94b7-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f94b7-151">privacyInformationUrl</span></span>|<span data-ttu-id="f94b7-152">String</span><span class="sxs-lookup"><span data-stu-id="f94b7-152">String</span></span>|<span data-ttu-id="f94b7-153">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="f94b7-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f94b7-154">关系</span><span class="sxs-lookup"><span data-stu-id="f94b7-154">Relationships</span></span>
|<span data-ttu-id="f94b7-155">关系</span><span class="sxs-lookup"><span data-stu-id="f94b7-155">Relationship</span></span>|<span data-ttu-id="f94b7-156">类型</span><span class="sxs-lookup"><span data-stu-id="f94b7-156">Type</span></span>|<span data-ttu-id="f94b7-157">描述</span><span class="sxs-lookup"><span data-stu-id="f94b7-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f94b7-158">categories</span><span class="sxs-lookup"><span data-stu-id="f94b7-158">categories</span></span>|<span data-ttu-id="f94b7-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)集合</span><span class="sxs-lookup"><span data-stu-id="f94b7-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="f94b7-160">此电子书的类别列表。</span><span class="sxs-lookup"><span data-stu-id="f94b7-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="f94b7-161">assignments</span><span class="sxs-lookup"><span data-stu-id="f94b7-161">assignments</span></span>|<span data-ttu-id="f94b7-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f94b7-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="f94b7-163">此电子书的分配列表。</span><span class="sxs-lookup"><span data-stu-id="f94b7-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="f94b7-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="f94b7-164">installSummary</span></span>|[<span data-ttu-id="f94b7-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f94b7-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="f94b7-166">移动应用安装摘要。</span><span class="sxs-lookup"><span data-stu-id="f94b7-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="f94b7-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="f94b7-167">deviceStates</span></span>|<span data-ttu-id="f94b7-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f94b7-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="f94b7-169">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="f94b7-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="f94b7-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="f94b7-170">userStateSummary</span></span>|<span data-ttu-id="f94b7-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f94b7-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="f94b7-172">此电子书的安装状态列表。</span><span class="sxs-lookup"><span data-stu-id="f94b7-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f94b7-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f94b7-173">JSON Representation</span></span>
<span data-ttu-id="f94b7-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f94b7-174">Here is a JSON representation of the resource.</span></span>
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




