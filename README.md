# Github-Storage-Abuse-Unique-files


mkdir -p unique_test

for i in $(seq -w 1 100); do
  head -c 2097152 </dev/urandom > "unique_test/file_${i}.bin"
done
