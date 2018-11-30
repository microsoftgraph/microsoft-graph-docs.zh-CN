---
title: registryKeyState 资源类型
description: 包含有关注册表的关键更改与通知，并更改的注册表项的过程信息。
ms.openlocfilehash: 37654aab2bf8f0afae0f7ec6ed544aed8634dacc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009510"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="ec522-103">registryKeyState 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec522-103">registryKeyState resource type</span></span>

<span data-ttu-id="ec522-104">包含有关注册表的关键更改与通知，并更改的注册表项的过程信息。</span><span class="sxs-lookup"><span data-stu-id="ec522-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="ec522-105">属性</span><span class="sxs-lookup"><span data-stu-id="ec522-105">Properties</span></span>

| <span data-ttu-id="ec522-106">属性</span><span class="sxs-lookup"><span data-stu-id="ec522-106">Property</span></span>     | <span data-ttu-id="ec522-107">类型</span><span class="sxs-lookup"><span data-stu-id="ec522-107">Type</span></span>        | <span data-ttu-id="ec522-108">说明</span><span class="sxs-lookup"><span data-stu-id="ec522-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ec522-109">配置单元</span><span class="sxs-lookup"><span data-stu-id="ec522-109">hive</span></span>|<span data-ttu-id="ec522-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="ec522-110">registryHive</span></span>|<span data-ttu-id="ec522-111">[Windows 注册表配置单元](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)中：</span><span class="sxs-lookup"><span data-stu-id="ec522-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="ec522-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="ec522-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="ec522-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="ec522-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="ec522-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="ec522-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="ec522-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="ec522-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="ec522-116">读</span><span class="sxs-lookup"><span data-stu-id="ec522-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="ec522-117">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="ec522-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="ec522-118">HKEY_USERS\\。默认值。</span><span class="sxs-lookup"><span data-stu-id="ec522-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="ec522-119">可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSamSoftware`、`localMachineSystem`、`usersDefault`。</span><span class="sxs-lookup"><span data-stu-id="ec522-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="ec522-120">Key</span><span class="sxs-lookup"><span data-stu-id="ec522-120">key</span></span>|<span data-ttu-id="ec522-121">字符串</span><span class="sxs-lookup"><span data-stu-id="ec522-121">String</span></span>|<span data-ttu-id="ec522-122">当前的 （即更改） 的注册表项 （排除配置单元）。</span><span class="sxs-lookup"><span data-stu-id="ec522-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="ec522-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="ec522-123">oldKey</span></span>|<span data-ttu-id="ec522-124">字符串</span><span class="sxs-lookup"><span data-stu-id="ec522-124">String</span></span>|<span data-ttu-id="ec522-125">（即更改之前） 以前注册表项 （排除配置单元）。</span><span class="sxs-lookup"><span data-stu-id="ec522-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="ec522-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="ec522-126">oldValueData</span></span>|<span data-ttu-id="ec522-127">字符串</span><span class="sxs-lookup"><span data-stu-id="ec522-127">String</span></span>|<span data-ttu-id="ec522-128">（即更改之前） 以前注册表项的值数据 （内容）。</span><span class="sxs-lookup"><span data-stu-id="ec522-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="ec522-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="ec522-129">oldValueName</span></span>|<span data-ttu-id="ec522-130">字符串</span><span class="sxs-lookup"><span data-stu-id="ec522-130">String</span></span>|<span data-ttu-id="ec522-131">（即更改之前） 以前注册表项的值名称。</span><span class="sxs-lookup"><span data-stu-id="ec522-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="ec522-132">操作</span><span class="sxs-lookup"><span data-stu-id="ec522-132">operation</span></span>|<span data-ttu-id="ec522-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="ec522-133">registryOperation</span></span>|<span data-ttu-id="ec522-134">更改的注册表项名称和/或值的操作。</span><span class="sxs-lookup"><span data-stu-id="ec522-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="ec522-135">可取值为：`unknown`、`create`、`modify`、`delete`。</span><span class="sxs-lookup"><span data-stu-id="ec522-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="ec522-136">processId</span><span class="sxs-lookup"><span data-stu-id="ec522-136">processId</span></span>|<span data-ttu-id="ec522-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ec522-137">Int32</span></span>|<span data-ttu-id="ec522-138">处理 ID (PID) 的过程的修改注册表项 （详细信息将显示通知进程集合中的过程）。</span><span class="sxs-lookup"><span data-stu-id="ec522-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="ec522-139">valueData</span><span class="sxs-lookup"><span data-stu-id="ec522-139">valueData</span></span>|<span data-ttu-id="ec522-140">字符串</span><span class="sxs-lookup"><span data-stu-id="ec522-140">String</span></span>|<span data-ttu-id="ec522-141">当前 （即更改） 的注册表项的值数据 （内容）。</span><span class="sxs-lookup"><span data-stu-id="ec522-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="ec522-142">数值名称</span><span class="sxs-lookup"><span data-stu-id="ec522-142">valueName</span></span>|<span data-ttu-id="ec522-143">字符串</span><span class="sxs-lookup"><span data-stu-id="ec522-143">String</span></span>|<span data-ttu-id="ec522-144">当前 （即更改） 的注册表项的值名称</span><span class="sxs-lookup"><span data-stu-id="ec522-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="ec522-145">valueType</span><span class="sxs-lookup"><span data-stu-id="ec522-145">valueType</span></span>|<span data-ttu-id="ec522-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="ec522-146">registryValueType</span></span>|[<span data-ttu-id="ec522-147">注册表项的值类型</span><span class="sxs-lookup"><span data-stu-id="ec522-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="ec522-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="ec522-148">REG_BINARY</span></span></li> <li><span data-ttu-id="ec522-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="ec522-149">REG_DWORD</span></span></li> <li><span data-ttu-id="ec522-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="ec522-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="ec522-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="ec522-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="ec522-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="ec522-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="ec522-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="ec522-153">REG_LINK</span></span></li> <li><span data-ttu-id="ec522-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="ec522-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="ec522-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="ec522-155">REG_NONE</span></span></li> <li><span data-ttu-id="ec522-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="ec522-156">REG_QWORD</span></span></li> <li><span data-ttu-id="ec522-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="ec522-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="ec522-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="ec522-158">REG_SZ</span></span></li></ul> <span data-ttu-id="ec522-159">可取值为：`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz`。</span><span class="sxs-lookup"><span data-stu-id="ec522-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec522-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec522-160">JSON representation</span></span>

<span data-ttu-id="ec522-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec522-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->