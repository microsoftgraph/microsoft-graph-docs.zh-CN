# <a name="registrykeystate-resource-type"></a><span data-ttu-id="67bfb-101">registryKeyState 资源类型</span><span class="sxs-lookup"><span data-stu-id="67bfb-101">registryKeyState resource type</span></span>

<span data-ttu-id="67bfb-102">包含有关注册表项的更改与提示，以及如何更改注册表项的信息。</span><span class="sxs-lookup"><span data-stu-id="67bfb-102">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="67bfb-103">属性</span><span class="sxs-lookup"><span data-stu-id="67bfb-103">Properties</span></span>

| <span data-ttu-id="67bfb-104">属性</span><span class="sxs-lookup"><span data-stu-id="67bfb-104">Property</span></span>     | <span data-ttu-id="67bfb-105">类型</span><span class="sxs-lookup"><span data-stu-id="67bfb-105">Type</span></span>        | <span data-ttu-id="67bfb-106">说明</span><span class="sxs-lookup"><span data-stu-id="67bfb-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="67bfb-107">hive</span><span class="sxs-lookup"><span data-stu-id="67bfb-107">Hive</span></span>|<span data-ttu-id="67bfb-108">registryHive</span><span class="sxs-lookup"><span data-stu-id="67bfb-108">registryHive</span></span>|<span data-ttu-id="67bfb-109"> [Windows 注册表配置单元](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)：</span><span class="sxs-lookup"><span data-stu-id="67bfb-109">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="67bfb-110">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="67bfb-110">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="67bfb-111">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="67bfb-111">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="67bfb-112">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="67bfb-112">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="67bfb-113">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="67bfb-113">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="67bfb-114">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="67bfb-114">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="67bfb-115">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="67bfb-115">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="67bfb-116">HKEY_USERS\\。默认值。</span><span class="sxs-lookup"><span data-stu-id="67bfb-116">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="67bfb-117">可取值为：`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSamSoftware`、`localMachineSystem`、`usersDefault`。</span><span class="sxs-lookup"><span data-stu-id="67bfb-117">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="67bfb-118">key</span><span class="sxs-lookup"><span data-stu-id="67bfb-118">key</span></span>|<span data-ttu-id="67bfb-119">字符串</span><span class="sxs-lookup"><span data-stu-id="67bfb-119">String</span></span>|<span data-ttu-id="67bfb-120">当前的 （更改后）的注册表项 （不含 HIVE）。</span><span class="sxs-lookup"><span data-stu-id="67bfb-120">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="67bfb-121">oldKey</span><span class="sxs-lookup"><span data-stu-id="67bfb-121">oldKey</span></span>|<span data-ttu-id="67bfb-122">字符串</span><span class="sxs-lookup"><span data-stu-id="67bfb-122">String</span></span>|<span data-ttu-id="67bfb-123">更改之前的注册表项 （不含 HIVE）。</span><span class="sxs-lookup"><span data-stu-id="67bfb-123">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="67bfb-124">oldValueData</span><span class="sxs-lookup"><span data-stu-id="67bfb-124">oldValueData</span></span>|<span data-ttu-id="67bfb-125">字符串</span><span class="sxs-lookup"><span data-stu-id="67bfb-125">String</span></span>|<span data-ttu-id="67bfb-126">此前（即更改之前）的注册表项的值数据 （内容）。</span><span class="sxs-lookup"><span data-stu-id="67bfb-126">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="67bfb-127">oldValueName</span><span class="sxs-lookup"><span data-stu-id="67bfb-127">oldValueName</span></span>|<span data-ttu-id="67bfb-128">字符串</span><span class="sxs-lookup"><span data-stu-id="67bfb-128">String</span></span>|<span data-ttu-id="67bfb-129">此前（即更改之前）注册表项的值名称。</span><span class="sxs-lookup"><span data-stu-id="67bfb-129">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="67bfb-130">operation</span><span class="sxs-lookup"><span data-stu-id="67bfb-130">operation</span></span>|<span data-ttu-id="67bfb-131">registryOperation</span><span class="sxs-lookup"><span data-stu-id="67bfb-131">registryOperation</span></span>|<span data-ttu-id="67bfb-132">更改的注册表项名称和/或值的操作。</span><span class="sxs-lookup"><span data-stu-id="67bfb-132">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="67bfb-133">可取值为：`unknown`、`create`、`modify`、`delete`。</span><span class="sxs-lookup"><span data-stu-id="67bfb-133">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="67bfb-134">processId</span><span class="sxs-lookup"><span data-stu-id="67bfb-134">processId</span></span>|<span data-ttu-id="67bfb-135">Int32</span><span class="sxs-lookup"><span data-stu-id="67bfb-135">Int32</span></span>|<span data-ttu-id="67bfb-136">修改注册表项流程的流程 ID (PID)（ 流程详细信息将显示于通知的 'process' 集合中）。</span><span class="sxs-lookup"><span data-stu-id="67bfb-136">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="67bfb-137">valueData</span><span class="sxs-lookup"><span data-stu-id="67bfb-137">valueData</span></span>|<span data-ttu-id="67bfb-138">字符串</span><span class="sxs-lookup"><span data-stu-id="67bfb-138">String</span></span>|<span data-ttu-id="67bfb-139">当前 （即更改后）的注册表项的值数据 （内容）。</span><span class="sxs-lookup"><span data-stu-id="67bfb-139">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="67bfb-140">valueName</span><span class="sxs-lookup"><span data-stu-id="67bfb-140">valueName</span></span>|<span data-ttu-id="67bfb-141">字符串</span><span class="sxs-lookup"><span data-stu-id="67bfb-141">String</span></span>|<span data-ttu-id="67bfb-142">当前 （即更改后）的注册表项的值名称</span><span class="sxs-lookup"><span data-stu-id="67bfb-142">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="67bfb-143">valueType</span><span class="sxs-lookup"><span data-stu-id="67bfb-143">ValueType</span></span>|<span data-ttu-id="67bfb-144">registryValueType</span><span class="sxs-lookup"><span data-stu-id="67bfb-144">registryValueType</span></span>|[<span data-ttu-id="67bfb-145">注册表项的值类型</span><span class="sxs-lookup"><span data-stu-id="67bfb-145">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="67bfb-146">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="67bfb-146">REG_BINARY</span></span></li> <li><span data-ttu-id="67bfb-147">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="67bfb-147">REG_DWORD</span></span></li> <li><span data-ttu-id="67bfb-148">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="67bfb-148">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="67bfb-149">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="67bfb-149">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="67bfb-150">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="67bfb-150">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="67bfb-151">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="67bfb-151">REG_LINK</span></span></li> <li><span data-ttu-id="67bfb-152">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="67bfb-152">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="67bfb-153">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="67bfb-153">REG_NONE</span></span></li> <li><span data-ttu-id="67bfb-154">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="67bfb-154">REG_QWORD</span></span></li> <li><span data-ttu-id="67bfb-155">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="67bfb-155">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="67bfb-156">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="67bfb-156">REG_SZ</span></span></li></ul> <span data-ttu-id="67bfb-157">可能的值为：`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz`。</span><span class="sxs-lookup"><span data-stu-id="67bfb-157">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67bfb-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67bfb-158">JSON representation</span></span>

<span data-ttu-id="67bfb-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67bfb-159">The following is a JSON representation of the resource.</span></span>

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